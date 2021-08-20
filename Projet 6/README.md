## Projet 6. Détectez des faux billets avec R ou Python

Mon client est une organisation publique ayant pour objectif de mettre en place des méthodes d’identification des contrefaçons des billets en euros. Dans le cadre de cette lutte, il souhaite mettre en place un algorithme qui soit capable de différencier automatiquement les vrais des faux billets. Lorsqu’un billet arrive, il a une machine qui consigne l’ensemble de ses caractéristiques géométriques. Au travers des années de lutte, il a observé des différences de dimensions entre les vrais et les faux billets. Ces différences sont difficilement notables à l’œil nu, mais une machine devrait sans problème arriver à les différencier.

Ainsi, il faudrait construire un algorithme qui, à partir des caractéristiques géométriques d’un billet, serait capable de définir si ce dernier est un vrai ou un faux billet. Dimensions géométriques :
* length : la longueur du billet (en mm) ;
* height_left : la hauteur du billet (mesurée sur le côté gauche, en mm) ;
* height_right : la hauteur du billet (mesurée sur le côté droit, en mm) ;
* margin_up : la marge entre le bord supérieur du billet et l'image de celui-ci (en mm) ;
* margin_low : la marge entre le bord inférieur du billet et l'image de celui-ci (en mm) ;
* diagonal : la diagonale du billet (en mm).

Il y a un fichier d’exemple contenant 1 500 billets, que j'utilise pour paramétrer mon algorithme. Parmi ces 1 500 billets, 1 000 sont vrais et 500 sont faux ; une colonne a été ajoutée pour vous préciser la nature du billet. Je teste de diverses méthodes de prédiction (une régression logistique classique, un k-means, une arbe de décisions, etc.) et j'analyse des nombres de faux positifs et faux négatifs via une matrice de confusion pour choisir la meilleure méthode.
