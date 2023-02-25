# Correction Flexbox Facile

## Exo 1

Voici le code qu'il fallait mettre :

![Voir l'image](./assets/img/Exo%201%20correction.png)

On cible tous simplement le container des boites `container-box`, et on active le display flex avec `display: flex;`.

*Petit rappel : par défaut, `display: flex;` met directement en ligne, donc pas besoin d'ajouter une autre propriété.*

## Exo 2

Voici la ligne qu'il fallait ajouter :

![Voir l'image](./assets/img/Exo%202%20correction.png)

Pour gérer l'axe X, il faut utiliser `justify-content`. En plus, on voit que les boites sont centrées, donc on ajoute simplement la valeur `center` : `justify-content: center;`.

## Exo 3

Voici l'autre ligne à ajouter :

![Voir l'image](./assets/img/Exo%203%20correction.png)

Pour gérer l'axe Y, il faut utiliser `align-items`. Il est également centré, donc on ajoute la valeur `center` également : `align-items: center;` 

## Exo 4

Voici le changement qu'il fallait faire :

![Voir l'image](./assets/img/Exo%204%20correction.png)

On reste sur un changement de placement dans l'axe X, on voit que les boites ne sont pas collée, et que l'espace entre les boites et bordure de page ne sont pas identiques, donc il nous reste une valeur pour ça `space-around`

Donc il suffit de remplacer la valeur de `justify-content` (axe X) : `justify-content: space-around;`

## Exo 5

Voici le changement qu'il fallait faire :

![Voir l'image](./assets/img/Exo%205%20correction.png)

On reste encore sur un changement de placement dans l'axe X, on voit que les boites sont collées contre les bordures et que les marges aux milieux sont répartie de façon égale. On a donc utilisé la valeur `space-between`.

Donc il suffit encore une fois de remplacer la valeur de `justify-content` (axe X) : `justify-content: space-between;`

## Exo 5 (BONUS)

Voici la ligne à ajouter pour ce bonus :

![Voir l'image](./assets/img/Exo%205%20correction%20bonus.png)

Dans ce cas-là, on voit que les boites sont inversées niveau couleur (effet miroir), que la 1er est dernière, la 2éme est avant-dernière etc...

On est donc sur un changement de direction...

> Il existe une propriété en flex pour ça, flex-direction non ?

Exact ! il suffit donc juste d'ajouter la propriété `flex-direction` et d'y ajouter une valeur.

> Vu que les boites sont toujours en ligne, donc je pense qu'il y a un row quelques chose dedans, non ? 

Bien vu, row est par défaut, dans l'ordre qu'il est implanté en HTML (si on avait mis 1 2 3 4 on aurait 1 2 3 4 en sortie sur notre écran, ce qui est normal)

Donc il suffit d'ajouter la valeur `row-reverse` pour *renverser* l'ordre (passer de **1 2 3 4** à un ordre inversé **4 3 2 1**) : `flex-direction: row-reverse;`

## Exo 6

Voici la ligne qu'il fallait ajouter (ou modifier si vous aviez fait le bonus) :

![Voir l'image](./assets/img/Exo%206%20correction.png)

On change la direction de notre container de boites, on passe de ligne *row* a *column*.

Donc il suffit d'ajouter cette valeur : `flex-direction: column;`

## Exo 7

Voici la ligne qu'il fallait modifier :

![Voir l'image](./assets/img/Exo%207%20correction.png)

> Alors là je ne comprends plus, on est sur un axe horizontal et pourtant on doit mofidier un axe vertical avec align-items en ajoutant la valeur "end".

Oui ça peut parraître troublant au début quand on ne comprends pas trop dans quel sens on se trouve. 

Faisons les choses dans l'ordre, de base la page commence en haut et fini en bas, donc si les mêmes valeurs sont ajouté sans `flex-direction: column;` on aurait nos boites tout en bas de notre page. **(commente la ligne `flex-direction: column;` dans ton CSS pour voir de tes propres yeux le comportement)**

Et si on utilise le `flex-direction` on change donc de **direction**. On commence à comprendre que la page démarre de la gauche et fini à droite. Si on met la valeur `start` à notre `flex-direction` on se rend compte qu'elle commence bien à gauche.

Donc pour qu'elle soit à droite on utilise : `align-items: end;`

*Si on bascule notre écran de 90 degrès dans le sens des aiguilles d'une montre, on constate que le `align-items: end;` est bien notre axe Y à modifier et que la valeur `end` correspond au bas de notre écran*