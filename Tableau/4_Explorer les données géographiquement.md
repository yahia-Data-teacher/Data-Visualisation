# Explorer vos données géographiquement

Vous avez créé une vue efficace qui vous permet d'analyser les ventes et les profits par produit sur plusieurs années. Et après avoir examiné les ventes de produits dans la région South, vous décidez d'étudier les tendances et les caractéristiques dans cette région.

Étant donné que vous examinez des données géographiques (champ Région), vous avez la possibilité de créer une carte. Les cartes sont un moyen idéal d'afficher et d'analyser ce type d'informations. Et en plus, elles ont belle allure.

Pour cet exemple, Tableau a déjà affecté le rôle géographique approprié aux champs Pays, État, Ville et Code postal. car il a reconnu que chacun de ces champs contenait des données géographiques. Vous pouvez donc vous mettre à créer d'emblée votre vue Carte.

## Créer une carte
Repartez à zéro avec une nouvelle feuille de calcul.

1. Dans la partie inférieure de l'espace de travail, cliquez sur l'icône Nouvelle feuille de calcul.

![explore17](https://user-images.githubusercontent.com/73080397/204165396-3b5a9867-9ecf-4835-8e5e-549aa3ffbbc7.png)

Tableau conserve votre précédente feuille de calcul et en crée une nouvelle afin que vous puissiez continuer à explorer vos données sans perdre votre travail.

2. Dans le volet Données, double-cliquez sur State pour l'ajouter à Detail dans la fiche Repères.

Vous avez maintenant une carte !

![Explore3](https://user-images.githubusercontent.com/73080397/204165427-8d1ff91d-0add-4850-8ce2-880fc9e3170e.gif)

Étant donné que Tableau sait déjà que les noms d'État sont des données géographiques, et parce que le rôle géographique État/province est attribué à la dimension État, Tableau crée automatiquement une carte.

Il existe un repère pour chacun des 48 États continus dans votre source de données. (L'Alaska et Hawaï ne sont malheureusement pas inclus dans votre source de données, donc ils sont laissés de côté.)

Notez que le champ Country est également ajouté à la vue. Cela s'explique par le fait que les champs géographiques dans Sample - Superstore font partie d'une hiérarchie. Chaque niveau de la hiérarchie est ajouté en tant que niveau de détail.

De plus, les champs Latitude et Longitude sont ajoutés aux étagères Colonnes et Lignes. Vous pouvez y penser comme à des champs X et Y. Ils sont essentiels à chaque fois que vous souhaitez créer une carte parce que chaque lieu dans vos données est associé à une valeur de latitude et de longitude. Il arrive parfois que les champs Latitude et Longitude soient générés par Tableau. D'autres fois, il vous faudra peut-être les inclure manuellement dans vos données. Vous trouverez des ressources complémentaires à ce sujet dans la bibliothèque d'apprentissage.

Maintenant, c'est une chose d'avoir une jolie carte centrée sur 48 États, mais rappelons-nous que votre but était d'étudier ce qui se passe dans la région South.

3. Faites glisser Region sur l'étagère Filtres, puis filtrez jusqu'au niveau South uniquement. La carte effectue un zoom sur la région South (un repère pour chaque État, soit 11 au total).

Vous souhaitez maintenant voir comment vos données se présentent pour cette région, donc vous commencez à faire glisser d'autres champs vers la fiche Repères :

4. Faites glisser la mesure Sales vers Couleur sur la fiche Repères.

![Explore4](https://user-images.githubusercontent.com/73080397/204165469-366836ba-00a7-4cee-b044-96e4273ac0d3.gif)

La vue se met automatiquement à jour pour devenir une carte pleine, et attribue une couleur à chaque État en fonction de ses ventes totales. Étant donné que vous explorez les ventes de produits, vous souhaitez que vos ventes apparaissent en USD. Cliquez sur le champ Sum(Sales) sur l'étagère Colonnes et sélectionnez Format. Pour Nombres, sélectionnez Devise.

Chaque fois que vous ajoutez une mesure continue qui contient des nombres positifs (par exemple des ventes) à Couleur sur la fiche Repères, votre carte pleine se colore en bleu. Les valeurs négatives sont associées à la couleur orange.

Il peut arriver que vous ne souhaitiez pas du bleu pour votre carte. Vous préférez peut-être le vert, ou vos données traitent de sujets qui ne devraient pas être représentés par la couleur bleu, par exemple les feux de forêt ou les embouteillages. Cela pourrait porter à confusion.

Aucun souci, vous pouvez modifier la palette de couleurs comme vous le faisiez précédemment.

5. Cliquez sur Couleur sur la fiche Repères et sélectionnez Modifier les couleurs.

Pour cet exemple, vous voulez voir quels États sont performants et quels États affichent des ventes médiocres.

6. Dans la liste déroulante Palette, sélectionnez Rouge-vert divergent et cliquez sur OK. Vous pourrez ainsi distinguer rapidement les bons élèves et les mauvais élèves.

Votre vue se met à jour comme suit :

![Explore5](https://user-images.githubusercontent.com/73080397/204165531-adfb12d3-eb76-4d95-afce-19791e1fbdb1.png)

Un instant ! Tout est devenu rouge ! Que s'est-il passé ?

Les données sont exactes, et techniquement, vous pouvez comparer les mauvais élèves et les bons élèves, mais est-ce que cela recouvre toute la réalité ?

Les ventes sont-elles à ce point désastreuses dans certains États, ou y a-t-il simplement plus de personnes en Floride qui cherchent à acheter vos produits ? Peut-être avez-vous des magasins plus petits ou moins de magasins dans les États qui s'affichent en rouge. Ou alors les États qui s'affichent en vert ont une densité de population plus élevée, donc il y a tout simplement davantage d'acheteurs pour vos produits.

Quoi qu'il en soit, vous n'allez pas montrer cette vue à votre responsable car vous n'êtes pas sûr que les données présentent une histoire utile.

7. Cliquez sur l'icône Annuler dans la barre d'outils pour revenir à la jolie vue bleue.

Il reste toutefois un problème de couleur. Tout a l'air parfait. Voilà le problème.

À première vue, il semble que la Floride affiche les meilleurs résultats. Pointer sur son repère révèle un total de ventes de 89 474 USD, par rapport à la Caroline du Sud, par exemple, qui n'obtient que 8 482 USD de ventes. Par contre, l'un des États de la région South a-t-il été profitable ?

8. Faites glisser Profit sur Couleur sur la fiche Repères pour voir si vous pouvez répondre à cette question.

![Explore6](https://user-images.githubusercontent.com/73080397/204165564-0e7ee715-5119-4dca-a64a-7197948f92eb.png)

Voilà qui est mieux ! Le profit consistant souvent à la fois en valeurs positives et négatives, Tableau sélectionne automatiquement la palette de couleurs divergente Orange-bleu pour afficher rapidement les États associés à un profit négatif et ceux associés à un profit positif.

Il apparaît maintenant clairement que le Tennessee, la Caroline du Sud et la Floride ont un profit négatif, bien qu'ils aient de bons chiffres, et même d'excellents chiffres de vente. Alors pourquoi ? Vous allez répondre à cette question à l'étape suivante.

## Vérifiez votre travail ! Découvrez « Créer une carte » en action

![explore18](https://user-images.githubusercontent.com/73080397/204165592-7b8b619a-9110-4b92-8440-0053cd94ff0c.gif)

