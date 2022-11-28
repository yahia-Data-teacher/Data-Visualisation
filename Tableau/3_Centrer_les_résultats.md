# 3. Centrer les résultats

Vous avez créé une vue de ventes de produits représentée par catégorie et sous-catégorie. Vous progressez, mais il reste beaucoup de données à trier. Vous avez besoin d'identifier facilement les points de données intéressants et de vous concentrer sur des résultats spécifiques. Cela tombe bien, Tableau propose des options fort utiles.

Vous pouvez utiliser les filtres et les couleurs pour vous centrer sur les détails qui vous intéressent. Après avoir effectué cette mise au point, vous pouvez commencer à utiliser d'autres fonctions Tableau Desktop pour interagir avec les données.

## Ajouter des filtres à votre vue

Vous pouvez utiliser des filtres pour inclure ou exclure des valeurs dans votre vue. Dans cet exemple, vous décidez d'ajouter deux filtres simples à votre feuille de calcul afin de faciliter l'analyse des ventes de produits par sous-catégorie pour une année spécifique.

1. Dans le volet Données, faites un clic droit sur Order Date et sélectionnez Afficher le filtre.

2. Répétez l'étape ci-dessus pour le champ Sub-Category.

Les filtres sont ajoutés sur le côté droit de votre vue dans l'ordre dans lequel vous les avez sélectionnés. Les filtres sont des types de fiches et peuvent être déplacés sur le canevas en cliquant sur le filtre et en le déposant sur un autre emplacement de la vue. Lorsque vous déplacez le filtre, une ligne apparaît et vous indique où vous pouvez déposer le filtre pour le déplacer.

![Drag10](https://user-images.githubusercontent.com/73080397/204225503-1ec5fe1b-5c46-48d0-b0bc-0c0c348374c1.png)

## Vérifiez votre travail ! Découvrez « Appliquer des filtres à votre vue » en action

![Drag25](https://user-images.githubusercontent.com/73080397/204225601-41acaba0-61a7-4747-8ac7-0e3d34015748.gif)

## Ajouter de la couleur à votre vue

L'ajout de filtres vous aide à trier toute cette masse de données. Mais que de bleu ! Il est temps de remédier à cette situation.

Pour le moment, vous êtes en train de contempler les totaux de vente pour vos différents produits. Vous pouvez voir que certains produits ont toujours des ventes faibles et que certains produits peuvent être de bons candidats à la réduction des efforts de vente pour ces gammes de produits. Mais à quoi ressemble la rentabilité globale de vos différents produits ? Faites glisser Profit sur Couleur pour voir ce qui se passe.

Depuis le volet Données, faites glisser Profit vers Couleur sur la fiche Repères.

En faisant glisser Profit sur Couleur, vous voyez maintenant apparaître des pertes pour les tables, les bibliothèques et même les machines. Vous venez de révéler une autre information !
![Dragcolor1](https://user-images.githubusercontent.com/73080397/204225667-dfc978e0-3963-4734-a313-1ff4ab1aec60.png)

## Vérifiez votre travail ! Découvrez « Ajouter de la couleur à votre vue » en action

![Drag26](https://user-images.githubusercontent.com/73080397/204225720-0c3f7eaf-8c8b-494c-9549-bb90736d6d56.gif)

## Trouver les informations clés
Comme vous l'avez appris, vous pouvez explorer vos données à mesure que vous créez des vues avec Tableau Desktop. L'ajout de filtres et de couleurs vous aide à mieux visualiser vos données et à identifier d'emblée les problèmes.

L'étape suivante consiste à interagir avec votre vue pour que vous puissiez commencer à dessiner vos conclusions.

À l'analyse de votre vue, vous avez pu constater qu'il y avait des produits non profitables, mais maintenant, vous voulez voir si ces produits l'ont été année après année.

Il est temps de sortir vos filtres pour examiner la question de plus près.

1. Dans la vue, dans la fiche de filtre Sub-Category, désélectionnez toutes les cases à cocher, sauf Bookcases, Machines, et Tables.

![FocusFilter1](https://user-images.githubusercontent.com/73080397/204225810-1a47aa0a-1f42-413d-b2e8-07cf973ed955.png)

Vous pouvez maintenant voir que, certaines années, les produits Bookcases et Machines étaient en fait profitables. Par contre, les Machines ont récemment cessé d’être rentables. Maintenant que vous avez fait une découverte importante, vous souhaitez collecter davantage d'informations avant de proposer un plan d'action à votre responsable.

Vous décidez, sur une intuition, de représenter votre vue par région :

2. Sélectionnez Tout dans la fiche de filtre Sub-Category pour afficher à nouveau toutes les sous-catégories.

3. Depuis le volet Données, faites glisser Region vers l'étagère Lignes et placez-le à droite de Sum(Sales).

Tableau crée une vue comportant plusieurs axes répartis par région.

![FocusRegions1](https://user-images.githubusercontent.com/73080397/204225936-950ef381-2a22-419d-af85-1ff978666206.png)

Vous voyez maintenant les ventes et la rentabilité par produit dans chaque région. En ajoutant une région à la vue et en filtrant la sous-catégorie sur Machines uniquement, vous remarquez que les machines dans la région South affichent des pertes générales plus élevées que dans vos autres régions. Vous avez mis à jour une information cachée !

![Focus_MachineSpike](https://user-images.githubusercontent.com/73080397/204226008-34e07899-0a2c-42af-8bbf-23d1dbc11abf.png)

Cette vue est celle qui intègre le mieux le travail que vous avez réalisé jusqu'à ce stade. Sélectionnez Tout dans la fiche de filtre Sub-Category (si vous avez modifié votre filtre) pour afficher à nouveau toutes les sous-catégories, nommer la feuille de calcul et ajouter un titre.

4. Dans la partie inférieure gauche de l'espace de travail, double-cliquez sur Feuille 1 et saisissez Sales by Product/Region.

Vous choisissez de centrer votre analyse sur la région South, mais vous ne souhaitez pas perdre la vue que vous avez créée. Dans Tableau Desktop, vous pouvez dupliquer votre feuille de calcul de manière à reprendre là vous vous étiez arrêté.

5. Dans votre classeur, faites un clic droit sur la feuille Sales by Product/Region et sélectionnez Dupliquer.

6. Renommez la feuille dupliquée en Sales in the South.

7. Dans votre nouvelle feuille de calcul, depuis le volet Données, faites glisser Region vers l'étagère Filtres pour l'ajouter en tant que filtre dans la vue.

8. Dans la boîte de dialogue de filtrage de la région, décochez toutes les cases sauf South, puis cliquez sur OK.

Votre vue se met à jour comme suit.

![FocusSouth1](https://user-images.githubusercontent.com/73080397/204226157-09c6f1c6-bdcf-4fc5-ac39-bf262ed879fa.png)

Vous pouvez maintenant vous centrer sur les ventes et le profit dans la région South. Vous voyez immédiatement que les ventes de machines affichent des pertes en 2018 et à nouveau en 2021. Ce sont des résultats qu'il faut passer au crible !

4. Enregistrez votre travail en sélectionnant Fichier > Enregistrer sous. Donnez un nom à votre classeur, par exemple Regional Sales and Profits.

## Vérifiez votre travail ! Découvrez « Trouver les informations clés » en action ci-dessous

![Drag27](https://user-images.githubusercontent.com/73080397/204226361-4127fc2c-f82c-4052-a8e1-a4b2f207e242.gif)

## Résumé de l'étape

Dans cette étape, vous avez utilisé les filtres et les couleurs pour travailler plus facilement avec vos données. Vous avez également découvert quelques fonctions amusantes Tableau qui vous aident à répondre à des questions clés sur vos données. Vous avez appris comment :

* Appliquer des filtres et des couleurs pour vous centrer facilement sur les domaines de vos données qui vous intéressent le plus.

* Interagit avec votre graphique en utilisant les outils fournis par Tableau.

* Dupliquer des feuilles de travail et enregistrer vos modifications pour continuer à explorer vos données de différentes manières sans perdre votre travail.

Une fois que vous avez exploré vos données dans Tableau Desktop, vous avez identifié les domaines qui vous intéressent. Vous savez que les ventes et le profit de la région South sont un problème, mais vous n'avez pas encore la solution. Vous souhaitez rechercher d'autres facteurs susceptibles d'expliquer ces résultats ? Vous allez ensuite utiliser une autre fonction clé de Tableau pour exploiter les données géographiques.

