# td-polytech-vercel
4- vercel -v
5- vercel init angular
6- cd angular puis vercel
7- vercel ls
8- vercel logs vercel-angular.maximeall.vercel.app
9- vercel inspect vercel-angular.maximeall.vercel.app

Inspect nous donne les informations du déploiement du projet.

10- Les variables d'environnement nous permettent d'injecter au projet des valeurs qu'on ne peut pas donner directmeent dans le code source et qui permettent de faire évoleur le comportement du projet en fonction de l'environnement dans lequel on le met en production.

11- vercel env add plain PASSWORD production
12- vercel env ls

13- Les variables secrètes sont cryptées et sont employées pour des usages particuliers comme des mots de passes ou des tokens d'accès. Elles sont un moyen de stocker de façon sécurisée des informations privées entre les déploiements.

14- vercel secret add username maxime, puis vercel env add secret USERNAME production avec le "username" secret de la première commande

16- Vercel met à disposition 3 types : Production, preview et dévelopment. Ces variables permettent de séparer les variables d'environnement selon l'avancée du projet. On peut donner un exemple simple d'une variable comme le chemin vers une base de données, modifiable pendant la phase de développement, mais qui n'a pas besoin d'être variable dans un environnement en production. On lui assigne donc une valeur définie en production, mais pas en développement.

18- 

19- Une pull request prmet de travailler sur une branche secondaire du projet puis de demander au propriétaire un merge sur la branche principale. Ici, Vercel la génère automatiquement pour l'environnement de preview.

20- Vercel edéploie la branche fusionnée dans l'environnement de production.
21- L'environnement de production correspond à la branche master du git. Utiliser des pull requests permet de développer le projet sans avoir à s'inuiéter dee conflits avec la branche principale du projet lors d'un push.

Une nouvelle feature est développée sur une nouvelle branche du git. Vercel la passe en environnement "devlopment". Lorsqu'elle est prête, Vercel effectue une pull request qui la fait passer en preview. Si la feature est acceptée, la nouvelle branche fusionne avec la branche principale dans l'environnement de prodction de Vercel.

22- Le serverless est un mode de fonctionnement où un fournisseur de serveur ou de cloud fournit des ressources à la demande d'une application. Le nom "serverless" est en fait détourné car on utilise un serveur, mais le développeur du projet n'a pas a se soucier de la gestion du serveur en lui-même; L'inétrêt principal de ce fonctionnement est de pouvoir mettre l'application en production très facilement, même en temps de développement. En général, cela permet même de réduire les coûts de développement en évitant de prendre son propre serveur pour toute la phase de développement.
