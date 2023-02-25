## Correction flexbox moyen

## Exo 1

Pour commencer, il faut l'activer comme d'habitude.

![Voir l'image](./assets/img/Exo%201%20correction.png)

Donc on cible bien les élèments qui contient les boites `content-box` et on lui met la propriété et la valeur `display: flex;`

## Exo 2

La ligne a ajouté est un `align-items`, on centre dans l'axe Y nos boites respective `content-box`.

![Voir l'image](./assets/img/Exo%202%20correction.png)

> Mais comment ça se fait ?

Dans le code déjà mis, on voit que `content-box` à une largeur mais également une hauteur. Donc les boites vont se centrer chacune dans leur container respectif de `content-box`.

## Exo 3

Là, on ajoute la propriété de l'axe X `justify-content`

![Voir l'image](./assets/img/Exo%203%20correction.png)

> Trop facile

Cela centrera les boites sur l'axe X dans leur propres container `content-box`

## Exo 4

La il y avait une subtilité à voir à l'oeil... l'espacement des marges. On a donc utilisé un `space-evenly`.

![Voir l'image](./assets/img/Exo%204%20correction.png)

> J'ai faillis mettre space-around...

Un `space-evenly` à le même espacement entre les bordures de page et les éléments, alors qu'un `space-around` en revanche, lui aura le même espace entre les éléments **mais** la marge de bordure de page sera plus ou moins important selon la place qu'il restera (divisé par 2).

## Exo 5

Comme dans l'exercice facile en bonus, ce n'est qu'un simple changement de direction. Donc on utilise `flex-direction`.

![Voir l'image](./assets/img/Exo%205%20correction.png)

> Easy !!!

Dans ce cas, la valeur est en ligne *row* et inversé *reverse* donc il fallait mettre : `flex-direction: row-reverse;` 

## Exo 6

Le dernier était un peu plus subtil, d'où le fait de pensez "boite" tout le temps en flex.

Dans ce cas, il fallait changer de boite pour jouer avec les propriétés.

`display: flex;`
`flex-direction: column-reverse;`

![Voir l'image](./assets/img/Exo%206%20correction.png)

> Oh my god !! j'ai réussi en pensant "boite"

On voit que les deux lignes se sont inversé sur l'image, donc on sait d'office qu'on ne serra plus dans le container des boites `content-box` car elles sont en ligne avec le `display: flex;`, donc on va devoir monter un cran encore au-dessus qui lui contient ces deux boites content-box pour agir dessus. 

Il s'agit donc de `container-box`

Pour activer le flex on utilise comme toujours: `display: flex;`

Et pour du coup inverser la direction qui est en column par défaut (block car ce sont des div) on fait : `flex-direction: column-reverse;`