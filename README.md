# My portfolio

## Projet 4. Réalisez une étude de santé publique avec R ou Python

Le projet est de créer un panorama de l’état de la malnutrition dans le monde, à partir des données de la FAO pour l’année 2017. Cette analyse comprend l'évaluation entre autres des paramètres suivants :
* la proportion de personnes en état de sous-nutrition ;
* le nombre théorique de personnes qui pourraient être nourries (idem pour la disponibilité alimentaire des produits végétaux) ;
* l’utilisation de la disponibilité intérieure ;
* les pays pour lesquels la proportion de personnes sous-alimentées est la plus forte ;
* les pays qui ont le plus bénéficié d’aide depuis 2013 ;
* les pays ayant le plus/le moins de disponibilité/habitant.

## Projet 5. Optimisez la gestion des données d'une boutique avec R ou Python

Cette mission se passe en 3 points :

1. Rapprocher deux exports : un export de l’ERP contenant les références produit, leur prix de vente et leur état de stock, et un export d’une table de l’outil de CMS contenant les informations des produits commercialisés en ligne (nom, description, nombre de ventes...). L’export issu de la boutique en ligne contient le nombre de ventes pour chaque produit depuis sa mise en ligne, il ne permet pas d’analyser l'évolution des ventes dans le temps.

2. Calcul du chiffre d’affaires par produit, ainsi que du total du chiffre d’affaires réalisé en ligne.

3. Effectuer une analyse sur la variable "Prix du produit" afin de détecter d’éventuelles valeurs aberrantes, de les lister et d’en faire une représentation graphique pour plus de lisibilité.

## Projet 6. Analysez les ventes d'une librairie avec R ou Python

Cette analyse est découpée en deux parties :

1. Une analyse des différents indicateurs de vente (mission de Antoine) :
* de différents indicateurs et graphiques autour du chiffre d'affaires, avec notamment l’évolution dans le temps ;
* un zoom sur les références, pour voir un peu les tops et les flops, la répartition par catégorie, etc ;
* quelques informations sur les profils des clients, et également la répartition du chiffre d'affaires entre eux, via une courbe de Lorenz.

2. Une analyse plus ciblée sur les clients (mission de Julie): l’objectif serait cette fois-ci de comprendre le comportement des clients en ligne, pour pouvoir ensuite comparer avec la connaissance acquise via les librairies physiques :
* le lien entre le genre d’un client et les catégories des livres achetés ;
* le lien entre l’âge des clients et le montant total des achats, la fréquence d’achat, la taille du panier moyen et les catégories des livres achetés ;
* la probabilité qu’un client achète la référence 0_525 sachant qu’il a acheté la référence 2_159.

## Projet 9. Produisez une étude de marché avec R ou Python

La poule qui chante est une entreprise française d’agroalimentaire. Elle souhaite se développer à l'international.

L'objectif de cette mission est de proposer une première analyse des groupements de pays que cette entreprise peut cibler pour exporter des poulets. Pour les buts de cette analyse je teste la classification ascendante hiérarchique, avec un dendrogramme comme visualisation. Ensuite j'utilise la méthode des k-means, afin d’affiner l’analyse et comparer les résultats des deux méthodes de clustering. Je réalise également une ACP afin de visualiser les résultats de mon analyse, comprendre les groupes, les liens entre les variables, les liens entre les individus.

## Projet 10. Détectez des faux billets avec R ou Python

L’Organisation nationale de lutte contre le faux-monnayage, ou ONCFM, est une organisation publique ayant pour objectif de mettre en place des méthodes d’identification des contrefaçons des billets en euros. Dans le cadre de cette lutte, ils souhaitent mettre en place un algorithme qui soit capable de différencier automatiquement les vrais des faux billets. Lorsqu’un billet arrive, ils ont une machine qui consigne l’ensemble de ses caractéristiques géométriques. Au travers des années de lutte, ils ont observé des différences de dimensions entre les vrais et les faux billets. Ces différences sont difficilement notables à l’œil nu, mais une machine devrait sans problème arriver à les différencier.

Ainsi, il faudrait construire un algorithme qui, à partir des caractéristiques géométriques d’un billet, serait capable de définir si ce dernier est un vrai ou un faux billet. Dimensions géométriques :

* length : la longueur du billet (en mm) ;
* height_left : la hauteur du billet (mesurée sur le côté gauche, en mm) ;
* height_right : la hauteur du billet (mesurée sur le côté droit, en mm) ;
* margin_up : la marge entre le bord supérieur du billet et l'image de celui-ci (en mm) ;
* margin_low : la marge entre le bord inférieur du billet et l'image de celui-ci (en mm) ;
* diagonal : la diagonale du billet (en mm).

Il y a un fichier d’exemple contenant 1 500 billets, que j'utilise pour paramétrer mon algorithme. Parmi ces 1 500 billets, 1 000 sont vrais et 500 sont faux ; une colonne a été ajoutée pour vous préciser la nature du billet. Je teste de diverses méthodes de prédiction (une régression logistique classique, un k-means, une arbe de décisions, etc.) et j'analyse des nombres de faux positifs et faux négatifs via une matrice de confusion pour choisir la meilleure méthode.

