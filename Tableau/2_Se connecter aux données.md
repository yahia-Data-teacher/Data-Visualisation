# 2. Se connecter aux données et créer une première vue
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


## Créer une vue

Vous êtes chargé d'identifier les principaux domaines à améliorer, mais par où commencer ? Sur la base de quatre années de données, vous décidez d'explorer les ventes générales pour voir ce que vous trouvez. Commencez par créer un graphique simple.

1. Depuis le volet Données, faites glisser Order Date vers l'étagère Colonnes.

*Remarque : lorsque vous faites glisser Order Date sur l'étagère des Colonnes, Tableau crée une colonne pour chaque année dans votre ensemble de données. Un indicateur Abc se trouve sous chaque colonne. Il indique que vous pouvez faire glisser du texte ou des données numériques ici, comme vous pourriez le voir dans un tableur Excel. Si vous faites glisser Sales vers cette zone, Tableau crée un tableau croisé (à la manière d'un tableur) et affiche les totaux de vente pour chaque année.

2. Depuis le volet Données, faites glisser Sales vers l'étagère Lignes.

Tableau génère le graphique suivant avec les ventes cumulées sous forme de somme (agrégées). Vous pouvez voir les ventes totales agrégées pour chaque année par date de commande.

![Drag1](https://user-images.githubusercontent.com/73080397/204230517-65c9b15f-9c31-4d06-a7ab-a90defbe5a4a.png)

Ce graphique en courbes montre que les ventes se portent bien et semblent augmenter dans la durée. C'est une bonne information, mais qui ne vous indique pas quels produits affichent les ventes les plus fortes, et si certains sont plus rentables que d'autres. Puisque vous venez juste de démarrer, vous décidez de continuer vos recherches pour dénicher d'autres informations

## Vérifiez votre travail ! Découvrez « Créer une vue » en action

![Drag23](https://user-images.githubusercontent.com/73080397/204230633-ab2fb4c6-80fa-4b7e-b4a4-40aaa9f4b733.gif)

## Affiner votre vue

Pour mieux analyser les produits qui dynamisent les ventes totales, essayez d'ajouter davantage de données. Commencez par ajouter les catégories de produit afin d'examiner les totaux de ventes sous un autre point de vue.

1. Depuis le Volet Données, faites glisser Category vers l'étagère Colonnes et placez-le à droite de YEAR(Order Date).
La vue est mise à jour sous forme d'un graphique à barres. En ajoutant une seconde dimension discrète à la vue, vous pouvez classer vos données en des tronçons discrets plutôt que d'examiner vos données en continu dans la durée. Un graphique à barres est généré et vous montre les ventes totales pour chaque catégorie de produit par an.


![Drag4](https://user-images.githubusercontent.com/73080397/204230737-3e4aabec-1d62-4313-9ad8-eefdaf6f9ef8.png)

Votre vue présente efficacement les ventes par catégorie (meubles, fournitures de bureau et technologie). Vous avez révélé des informations intéressantes.

Dans cette vue, vous pouvez voir que les ventes de meubles augmentent plus rapidement que les ventes de fournitures de bureau, bien que l'année 2021 ait été une très bonne année pour les fournitures de bureau. Peut-être pouvez-vous recommander que votre société concentre ses efforts commerciaux sur les meubles plutôt que sur les fournitures de bureau ? Votre société vend de nombreux produits différents dans ces catégories. Il vous faudra donc plus d'informations avant de pouvoir formuler une recommandation.

Pour vous aider à répondre à cette question, vous décidez d'examiner les produits par sous-catégorie pour voir quels articles se vendent le mieux. Par exemple, pour la catégorie des meubles, vous pouvez souhaiter voir des détails sur les bibliothèques, les chaises, les ameublements et les tables. L'analyse de ces données peut vous aider à analyser les ventes et ultérieurement, la profitabilité générale, donc ajoutez des sous-catégories à votre graphique à barres.

2. Double-cliquez sur Sub-Category ou faites-le glisser sur l'étagère Colonnes.
Remarque : vous pouvez faire un glisser-déplacer ou double-cliquer sur un champ pour l'ajouter à votre vue, mais faites attention. Tableau émet des hypothèses sur l'emplacement où ajouter ces données, et cet emplacement peut être différent de celui auquel vous vous attendez. Vous pouvez toujours cliquer sur Annuler pour supprimer le champ, ou le faire glisser hors de la zone où Tableau l'a placé et recommencer.

La sous-catégorie est un autre champ discret. Elle crée un autre en-tête au bas de la vue, et affiche une barre pour chaque sous-catégorie (68 fiches) représenté par catégorie et année.

![Drag9](https://user-images.githubusercontent.com/73080397/204230816-dbdaadf3-5c01-4127-af81-ed7319543126.png)

Vous avez bien progressé, mais il reste beaucoup de données à classer visuellement. Dans la section suivante, vous apprendrez à ajouter des couleurs, des filtres, et autres options permettant de mettre l'accent sur des résultats spécifiques.

## Vérifiez votre travail ! Découvrez « Affiner votre vue » en action

![Drag24](https://user-images.githubusercontent.com/73080397/204230964-f8686adb-5c3e-46a6-b423-afcdab4916b6.gif)

## Résumé de l'étape
Dans cette étape, votre but était de vous familiariser avec vos données et de les interroger pour les faire parler. Vous avez appris comment :

* Créer un graphique dans une vue opérationnelle.

* Ajouter des champs pour obtenir le niveau de détail adapté dans votre vue.

Vous êtes maintenant prêt à vous concentrer sur vos résultats pour identifier des domaines de préoccupation plus spécifiques. Dans la section suivante, vous allez apprendre à utiliser les filtres et les couleurs pour explorer visuellement vos données.

