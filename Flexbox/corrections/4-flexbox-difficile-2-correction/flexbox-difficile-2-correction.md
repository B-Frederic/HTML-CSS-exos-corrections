# Correction exercice difficile 2

Alors ça s'est bien passé ?
> Bien évidement !

Super, voila donc le code (n'oublie pas que l'on peut faire ça différemment, le principal est d'avoir le même rendu):

![Voir l'image](./assets/img/Code%201.png)

![Voir l'image](./assets/img/Code%202.png)

Je ne pense pas avoir besoin de détailler le code, par contre tu peux voir que des fois il est bien de cumuler des class pour leur mettre les propriétés, je pense notamment au `main-box-1`, `main-box-2` et `main-box-3`.
Vu qu'elles ont toutes les mêmes propriétés flexbox et les mêmes valeurs, autant les cibler toutes les trois.

Il y a une petite subtilité, pour le `container-header`, on inverse les logos (Html et Css) avec `flex-direction: row-reverse;` mais on peut aussi tous simplement inversé les balises directement dans le code HTML

Pour le footer pareil, on peut inverser avec un `flex-direction: column-reverse;` ou aller dans le code Html et changé l'ordre des balises.

Mais tu l'as compris, le but là, était surtout de s'entrainer avec les flexbox.

> Oui, par contre j'ai remarqué autre chose, dans les dossiers il y a un fichier `anime.css` et dans mon code Html le lien est commenté ligne 8. C'est normal ?

J'allais y venir, comme tu l'as vue, le site comporte quelques effets de `transform`, les box, les boutons de lien (nav et aside) mais il y a également cet effet sympa sur les logos, c'est un peu la cerise sur le gâteau après avoir bossé dur pour refaire le site.

Je te laisse donc aller décommenter la ligne 8 dans ton Html, et regarder ce qui se passe avec les logos.

> Trop top, on peut vraiment tous faire en CSS !

Oui, et encore tu n'imagines pas l'étendu de ce qu'on peut faire avec.