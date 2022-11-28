# 6. Créer un tableau de bord 

Vous avez créé quatre feuilles de calcul qui transmettent des informations importantes à porter à la connaissance de votre responsable. Vous avez maintenant besoin d'un moyen de montrer les pertes dans le Tennessee, en Caroline du Nord et en Floride et d'expliquer certaines des raisons pour lesquelles les bénéfices sont faibles.

Pour cela, vous pouvez utiliser des tableaux de bord et afficher plusieurs feuilles de calcul à la fois, et, si vous le souhaitez, interagir avec elles.

## Configurer votre tableau de bord

Vous souhaitez mettre l'accent sur le fait que certains articles vendus dans certains lieux affichent des résultats médiocres. La vue en graphique à barres du profit et votre vue Carte démontrent ce point de manière éloquente.

1. Cliquez sur le bouton Nouveau tableau de bord.

![Build1](https://user-images.githubusercontent.com/73080397/204166952-174e7c38-74f8-4d64-b98b-b513dfc1be7d.png)

2. Dans le volet Tableau de bord sur la gauche, vous verrez les feuilles que vous avez créées. Faites glisser Sales in the South vers votre tableau de bord vide.

3. Faites glisser Profit Map vers votre tableau de bord et déposez-le en haut de la vue Sales in the South.

Votre vue se met à jour comme suit :

![Build2](https://user-images.githubusercontent.com/73080397/204167007-561835eb-da92-4e11-83ad-88984369e045.png)

Vous pouvez maintenant voir les deux vues à la fois !

Malheureusement, le graphique à barres est un peu entassé, ce qui n'aide pas votre responsable à comprendre vos données.

## Organiser votre tableau de bord

Les détails de chaque article dans la section Sub-Category ne sont pas très lisibles dans votre graphique à barres Sales in the South. De plus, parce que la vue contient une carte, nous pouvons probablement nous passer de la colonne South region dans le graphique Sales in the South.

En résolvant ces problèmes, vous aurez davantage de latitude pour communiquer les informations dont vous avez besoin.

1. Dans le graphique Sales in the South, faites un clic droit dans la zone de colonne sous l'en-tête de colonne State et désélectionnez Afficher l'en-tête.

![Build2 5](https://user-images.githubusercontent.com/73080397/204167064-d5440dcf-50e8-41d9-9a43-a519afda9f03.png)

2. Répétez ce processus pour l'en-tête de ligne Category.

![Build2 6](https://user-images.githubusercontent.com/73080397/204167078-71b2062c-e7f5-48dc-a800-fe73dced5935.png)

Vous avez maintenant masqué les colonnes et lignes superflues de votre tableau de bord tout en préservant la répartition de vos données. L'espace supplémentaire facilite la visualisation des données sur votre tableau de bord, mais éclaircissons encore plus les choses.

3. Faites un clic droit sur le titre Profit Map et sélectionnez Masquer le titre.

Le titre Profit Map n'apparaît plus dans le tableau de bord, ce qui libère encore plus d'espace.

4. Répétez cette étape pour le titre de la vue Sales in the South.

5. Sélectionnez la fiche de filtre Sous-Category sur le côté droit de votre vue, et en haut de la fiche, cliquez sur l'icône SupprimerIcône Supprimer du tableau de bord.

6. Répétez cette étape pour la seconde fiche de filtre Sub-Category et l'une des fiches de filtre Year of Order Date.

7. Cliquez sur la légende des couleurs Profit et faites-la glisser de la droite jusque sous le graphique Sales in the South.

8. Enfin, sélectionnez le filtre restant Year of Order Date, cliquez sur sa flèche déroulante, et sélectionnez Flottant. Déplacez-le vers l'espace blanc dans la vue Carte. Dans cet exemple, il est placé juste à proximité d'East Coast, dans l'Océan Atlantique.

Essayez de sélectionner différentes années en appliquant le filtre Year of Order Date. Vos données sont filtrées rapidement pour afficher les performances d'un État, année après année. C'est déjà bien, mais vous pourriez encore faciliter davantage la comparaison.

9. Cliquez sur la flèche déroulante en haut du filtre Year of Order Date, et sélectionnez Valeur unique (curseur).
Votre vue se met à jour comme suit :

![build6](https://user-images.githubusercontent.com/73080397/204167155-283cfa56-c160-4963-87e8-c8455d51e451.png)

Maintenant, votre tableau de bord a vraiment belle allure ! Vous pouvez maintenant comparer facilement le profit et les ventes par année. Mais cela n'est pas très différent de quelques images dans une présentation, et vous avez à votre disposition l'outil Tableau ! Rendons donc votre tableau de bord plus séduisant.

## Vérifiez votre travail ! Découvrez « Organiser votre tableau de bord » en action

![Build3](https://user-images.githubusercontent.com/73080397/204167182-a70fb69d-04fc-4241-8891-f4389bc46167.gif)

## Ajout d'interactivité

N'aimeriez-vous pas pouvoir afficher les sous-catégories profitables dans des États spécifiques ?

1. Sélectionnez Profit Map dans le tableau de bord et cliquez sur l'icône Utiliser comme filtreIcône Utiliser comme filtre en haut à droite.

2. Sélectionnez un État dans la région Sud de la carte.

Les ventes du graphique à barres South sont automatiquement mises à jour de manière à n'afficher que les ventes de sous-catégorie dans l'État sélectionné. Vous pouvez rapidement voir les sous-catégories profitables.

3. Cliquez sur une zone de la carte autre que les États du Sud colorés pour effacer votre sélection.

Vous souhaitez également que vos observateurs puissent voir le changement dans les profits en fonction de la date de commande.

4. Sélectionnez le filtre Year of Order Date, cliquez sur son menu déroulant et sélectionnez Appliquer aux feuilles de calcul > Feuilles de calcul sélectionnées.

5. Dans la boîte de dialogue Appliquer le filtre aux feuilles de travail, cliquez sur Tout sur le tableau de bord, puis cliquez sur OK.

Cette option indique à Tableau d'appliquer le filtre à toutes les feuilles de calcul du tableau de bord qui utilisent cette même source de données.

Explorez les performances d'un État par année à l'aide de votre nouveau tableau de bord interactif !

## Vérifiez votre travail ! Découvrez « Ajouter de l'interactivité » en action

Dans ce cas, nous filtrons les ventes réalisées dans la région South sur les articles vendus uniquement en Caroline du Nord, puis nous explorons le profit année par année.

![Build4](https://user-images.githubusercontent.com/73080397/204167212-87051056-4857-481f-af02-8eae08315577.gif)

## Renommer et accéder

Vous présentez votre tableau de bord à votre responsable qui l'apprécie beaucoup. Elle l'a appelé "Regional Sales and Profit", et vous faites de même en double-cliquant sur Tableau de bord 1 et en saisissant Regional Sales and Profit.

Dans ses recherches, votre responsable estime que la décision d'introduire des machines dans le marché de la Caroline du Nord en 2021 était une mauvaise idée.

Votre responsable se réjouit d'avoir ce tableau de bord à explorer, mais elle souhaite également que vous présentiez un plan d'action clair au reste de l'équipe. Elle vous demande de créer une présentation avec vos découvertes.

Heureusement pour vous, vous savez tout sur les histoires dans Tableau.


