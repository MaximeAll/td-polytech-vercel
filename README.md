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
