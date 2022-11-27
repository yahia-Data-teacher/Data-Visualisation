# 5. Filtrer

À l'étape précédente, vous avez découvert que le Tennessee, la Caroline du Nord et la Floride affichaient un profit négatif. Pour expliquer ces résultats, vous décidez d'explorer plus en détail et de vous centrer sur ces trois États.

## Aller au-delà de la vue Carte

Comme vous l'avez vu à la dernière étape, les cartes sont un excellent moyen de visualiser vos données sur une large échelle. Un graphique à barres vous aide à passer aux choses sérieuses. Pour cela, vous devez créer une autre feuille de calcul.

1. Double-cliquez sur Feuille 3 et nommez la feuille de calcul Profit Map.

2. Faites un clic droit sur la carte Profit Map au bas de l'espace de travail et sélectionnez Dupliquer. Nommez la nouvelle feuille Graphique à barres Negative Profit.

3. Dans la feuille de calcul Graphique à barres Negative Profit, cliquez sur Montre moi, puis sélectionnez barres horizontales.

La fonction Montre moi met en surbrillance différents types de graphiques en fonction des données que vous avez ajoutées à votre vue.

*Remarque : à tout moment, vous pouvez cliquer à nouveau sur Montre moi pour le réduire.*

![Explore8](https://user-images.githubusercontent.com/73080397/204165888-f7d35b53-8e46-49b2-9034-4f8423f223c7.png)

Vous avez maintenant à nouveau un graphique à barres, en un tournemain.

![Explore9](https://user-images.githubusercontent.com/73080397/204165919-5535a849-c835-4e33-9244-79e86683f141.png)

4. Pour sélectionner plusieurs barres sur la gauche, cliquez et faites glisser le curseur parmi les barres entre Tennessee, Caroline du Nord et Floride. Dans l'infobulle qui apparaît, sélectionnez Conserver uniquement pour vous centrer sur ces trois États.

*Remarque : Vous pouvez également cliquer avec le bouton droit de la souris sur les barres en surbrillance et sélectionner Conserver uniquement.*

Notez que le champ Inclusions pour État est ajouté à l'étagère des filtres pour indiquer que certains États sont exclus de la vue. L'icône à deux cercles sur le champ indique que le champ est un ensemble. Vous pouvez modifier ce choix en faisant un clic droit sur le champ dans l'étagère Filtres et en sélectionnant Modifier le filtre.

Vous voulez maintenant examiner les données pour les villes de ces États.

5. Dans l'étagère Lignes, cliquez sur l'icône plus dans le champ State pour explorer en cascade jusqu'au niveau de détail Ville.

Il y a presque trop d'informations ici, donc vous décidez de filtrer la vue jusqu'aux villes affichant le plus de pertes à l’aide d'un filtre N principaux.

## Vérifiez votre travail ! Découvrez les étapes 1-5 en action

![explore19](https://user-images.githubusercontent.com/73080397/204166032-1a20d3ef-2d98-4fb0-80cf-c854977dab44.gif)

Créer un filtre N principaux
Vous pouvez utiliser un filtre N principaux dans Tableau Desktop pour limiter le nombre de repères affichés dans votre vue. Dans ce cas, vous souhaitez utiliser le filtre N principaux pour identifier les villes les moins performantes.

1. Dans le volet Données, faites glisser City vers l'étagère Filtres.

2. Dans la boîte de dialogue Filtre, sélectionnez l'onglet Premiers, puis effectuez l'une des opérations suivantes :

  * a. Cliquez sur Par champ.
  * b. Cliquez sur la liste déroulante Premiers et sélectionnez Derniers pour faire apparaître les villes les moins performantes.
  * c. Saisissez 5 dans la zone de texte pour afficher les 5 villes les moins performantes de votre ensemble de données.

Tableau Desktop a déjà sélectionné un champ (Profit) et une agrégation (Somme) pour le filtre N principaux sur la base des champs de votre vue. Ces paramètres font en sorte que votre vue n'affiche que les cinq villes les moins performantes par somme de profit.

![Explore12](https://user-images.githubusercontent.com/73080397/204166213-e95ed974-b101-47f6-8bad-400c6f6e2b6a.png)

  * d. Cliquez sur OK.
 
Qu'est-il arrivé au graphique à barres et pourquoi est-il vide ? C'est une excellente question, et une bonne occasion de présenter l'ordre des opérations Tableau.

L'ordre des opérations de Tableau, également appelé encours de requêtes, désigne l'ordre dans lequel Tableau effectue diverses actions, par exemple l'ordre dans lequel il applique vos filtres à la vue.

Tableau applique les filtres dans l'ordre suivant :

1. Filtres d'extraits

2. Filtres de source de données

3. Filtres contextuels

4. Filtres N principaux

5. Filtres de dimensions

6. Filtres de mesures

L'ordre dans lequel vous créez des filtres ou les arrangez dans l'étagère Filtres n'a rien à voir avec l'ordre dans lequel Tableau applique ces filtres à votre vue.

La bonne nouvelle est que vous pouvez indiquer à Tableau de modifier cet ordre lorsque les filtres de votre vue génèrent un résultat inhabituel. Dans cet exemple, le filtre N principaux est appliqué aux cinq villes les moins performantes par somme de profit pour l'ensemble de la carte. Par contre, étant donné qu’aucune de ces villes ne se trouve dans le Sud, le graphique est vide.

Pour corriger le graphique, ajoutez un filtre au contexte. Tableau saura ainsi qu'il doit filtrer ce champ en premier, où qu'il se trouve dans l'ordre des opérations.

Mais quel champ allez-vous ajouter au contexte ? L'étagère Filtres contient trois champs : Region (un filtre de dimension), City (un filtre N principaux), et Inclusions (Country, State) (Country, State) (un ensemble).

Si vous examinez à nouveau l'ordre des opérations, vous savez que l'ensemble et le filtre N principaux sont appliqués avant le filtre de dimension. Mais savez-vous si le filtre N principaux ou le filtre défini est appliqué en premier ? Découvrons-le.


3. Dans l'étagère Filtres, faites un clic droit sur le champ City et sélectionnez Ajouter au contexte.

Le champ City devient gris et se déplace en haut de l'étagère Filtres, mais rien ne change dans la vue. Donc même si vous forcez Tableau à filtrer d'abord par City, le problème n’est pas résolu.

4. Cliquez sur Annuler.

5. Sur l'étagère Filtres, faites un clic droit sur l'ensemble Inclusions (Country, State) (Country, State) et sélectionnez Ajouter au contexte.

L'ensemble Inclusions (Country, State) (Country, State) devient gris et se déplace vers le haut de l'étagère Filtres. Et les barres sont revenues !

Vous êtes sur une piste ! Mais la vue contient six villes, dont Jacksonville, en Caroline du Nord, qui affiche un bénéfice. Pourquoi une ville affichant un bénéfice apparaîtrait-elle dans la vue alors que vous avez créé un filtre qui était supposé l'en exclure ?

Jacksonville, Caroline du Nord, est inclus parce que la ville est le niveau de détail le plus bas affiché dans la vue. Pour que Tableau Desktop puisse faire la différence entre Jacksonville, Caroline du Nord et Jacksonville, Floride, il faudrait que vous alliez jusqu'au niveau de détail suivant dans la hiérarchie des lieux, qui, dans ce cas, est le code postal. Après l’ajout du code postal, vous pouvez exclure Jacksonville en Caroline du Nord sans exclure en même temps Jacksonville en Floride.

6. Sur l'étagère Lignes, cliquez sur l'icône plus dans City pour explorer jusqu'au niveau de détail Code postal.

7. Faites un clic droit sur le code postal de Jacksonville, Caroline du Nord, 28540, puis sélectionnez Exclure.

Le code postal est ajouté à l'étagère des filtres pour indiquer que certains membres du champ Postal Code sont exclus de la vue. Même lorsque vous supprimez le champ Code postal de la vue, le filtre reste.

8. Faites glisser Code postal hors de l'étagère Lignes.

![Explore14](https://user-images.githubusercontent.com/73080397/204166310-6406b879-abb3-497f-a8e6-77c1a70305ae.png)

## Vérifiez votre travail ! Découvrez les étapes 1-8 en action

![Explore13](https://user-images.githubusercontent.com/73080397/204166327-c7a7037b-b40a-41ee-be7e-5c1a8379a23a.gif)

Maintenant que vous avez centré votre vue sur les villes les moins profitables, vous pouvez poursuivre votre investigation et identifier les produits responsables.

## Identifier les fauteurs de trouble

Vous décidez de découper la vue par sous-catégorie afin d'identifier les produits qui tirent le profit vers le bas. Vous savez que le champ Sub-Category contient des informations sur les produits vendus par lieu, donc c'est votre point de départ.

1. Faites glisser Sub-Category vers l'étagère Lignes, et placez-le à droite de City.

2. Faites glisser Profit vers Couleur dans la fiche Repères pour voir plus facilement les produits affichant un profit négatif.

3. Dans le volet Données, faites un clic droit sur Order Date et sélectionnez Afficher le filtre.

Vous pouvez maintenant explorer les profits négatifs pour chaque année si vous le souhaitez et repérer rapidement les produits à l'origine de pertes.

Les machines, les tables et les classeurs ne brillent pas par leurs résultats. Que diriez-vous de cesser de vendre ces articles à Jacksonville, Miami, Burlington, Knoxville et Memphis ?

![Explore15](https://user-images.githubusercontent.com/73080397/204166369-e15ca744-3247-46e5-a65d-f32ae8aa6012.png)

## Vérifier vos conclusions

L'élimination des classeurs, des machines et des tables va-t-elle redresser les profits en Floride, Caroline du Nord et Tennessee ? Pour le savoir, vous pouvez filtrer les produits problématiques pour voir ce qui se passe.

1. Revenez à votre vue Carte en cliquant sur l'onglet de la feuille Profit Map.

2. Dans le volet Données, faites un clic droit sur Sub-Category et sélectionnez Afficher le filtre.

Une fiche de filtre pour tous les produits que vous proposez apparaît en regard de la vue Carte. Vous utiliserez ce filtre plus tard.

3. Depuis le volet Données, faites glisser Profit et Profit Ratio sur Étiquette dans la fiche Repères. Pour formater le ratio de profit sous forme de pourcentage, cliquez avec le bouton droit de la souris sur le Profit Ratio et sélectionnez Format. Ensuite, pour Nombres par défaut, choisissez Pourcentage et définissez le nombre de décimales que vous souhaitez afficher sur la carte. Pour cette carte, nous choisirons zéro décimale.

Vous pouvez maintenant voir le profit exact de chaque État sans avoir à pointer le curseur dessus.

4. Dans le volet Données, faites un clic droit sur Order Date et sélectionnez Afficher le filtre pour ajouter un contexte à la vue.

Une fiche de filtre pour YEAR(Order Date) apparaît dans la vue. Vous pouvez maintenant voir le profit pour toutes les années ou une combinaison d'années, ce qui peut être utile pour votre présentation.

5. Désélectionnez Binders, Machines et Tables de la liste dans la fiche de filtre Sub-Category dans la vue.

Rappelez-vous que l'ajout de filtres à votre vue vous permet d'inclure ou d'exclure des valeurs pour mettre en exergue certaines parties de vos données;

À mesure que vous désélectionnez chaque membre, le profit pour le Tennessee, la Caroline du Nord et la Floride s'améliore, jusqu'à ce que chacun ait un profit positif à la fin.

![Explore16](https://user-images.githubusercontent.com/73080397/204166526-637e399b-c563-436e-9872-b07896de1863.gif)

Voici une découverte intéressante !

Il est clair que les classeurs, les machines et les tables sont responsables des pertes au Tennessee, en Caroline du Nord et en Floride, mais pas dans le reste de la région South. Vous remarquez comme le profit diminue dans certains autres États lorsque vous désélectionnez des articles dans la fiche de filtre ? Par exemple, si vous désactivez Binders dans la fiche de filtre Sub-Category, le profit chute de 4 % en Arkansas. Vous pouvez en déduire que les classeurs sont profitables en Arkansas.

Vous souhaitez partager cette découverte avec votre équipe en lui faisant retracer les mêmes étapes que vous.

6. Sélectionnez (Tout) dans la fiche de filtre Sub-Category de manière à inclure à nouveau tous les produits

## Vérifiez votre travail ! Découvrez « Vérifier vos conclusions » en action

![explore21](https://user-images.githubusercontent.com/73080397/204166588-f8f01de0-228a-4ebb-bd7d-1988a05c5c59.gif)

Vous savez maintenant que les machines, les tables et les classeurs sont des produits problématiques pour votre société. En vous concentrant sur la région South, vous voyez que ces produits ont un impact variable sur le profit. Cela peut faire l'objet d'une discussion intéressante avec votre responsable.

Vous allez ensuite rassembler le travail que vous avez effectué jusque-là dans un tableau de bord afin de pouvoir présenter vos conclusions avec clarté.

