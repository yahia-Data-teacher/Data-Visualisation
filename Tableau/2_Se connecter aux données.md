# 2. Se connecter aux données 
Tableau peut se connecter à toutes les sources de données accessibles qui sont largement utilisées. Il peut se connecter à des fichiers Excel, des fichiers PDF, des fichiers texte, etc. Il peut également se connecter à diverses bases de données en utilisant son connecteur ODBC. Tableau peut se connecter à des connecteurs web et à des serveurs.

Les connecteurs natifs de Tableau peuvent se connecter aux types de sources de données suivants :

* Systèmes de fichiers : Tels que Microsoft Excel, CSV, etc.
* Systèmes en nuage : Tels que Google bigQuery, Windows Azure, etc.
* Système relationnel : Tels que Microsoft SQL Server, Oracle, DB2, etc.
* Autres sources : Il utilise ODBC.

L'image ci-dessous montre toutes les sources de données disponibles via les connecteurs de données natifs de Tableau:

![data-connection-with-data-sources](https://user-images.githubusercontent.com/73080397/203032265-e8ef04c8-9841-471a-996a-78ec92c1eec2.png)


Pour le cas de tableau public, toutes ces options de connexion aux données ne sont pas disponibles:

![tableau_public](https://user-images.githubusercontent.com/73080397/203034907-a4865d32-27ca-47ce-874d-af531bd679a3.PNG)


Nous allons donc nous connecter aux données que nous allons télécharger : 
* Télecherger les données à partir de [ce lien](https://public.tableau.com/app/sample-data/sample_-_superstore.xls)
* Dans le volet de connexion, cliquer sur Microsoft Excel, et ouvrez le fichier téléchatgé sample_-_superstore.xls
* Trois tableaux s'affichent : Orders, People, et Returns :

![image](https://user-images.githubusercontent.com/73080397/203958839-778e664c-ca8a-4738-9b3d-98f96c9ecd5a.png)

* Faire glisser les trois tableaux, remarquer que les liaisons sont faites automatiquement :

![image](https://user-images.githubusercontent.com/73080397/203960203-b20460d7-c0b9-4f98-849f-aa913bab576b.png)

*Question : Par quelles clés les liaisons sont-elles faites entre les tableaux ?* 

#### Bonus : Différence entre  les produits Tbleau et logigramme pour choisir le produit adéquat
https://www.edureka.co/blog/tableau-desktop-vs-tableau-public-vs-tableau-reader/#:~:text=Tableau%20Desktop%20is%20meant%20for,%2C%20bloggers%2C%20students%20and%20more. 
