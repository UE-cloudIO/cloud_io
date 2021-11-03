# cloud_IO

Cloud_io est un jeux multijoueur crée sur unreal Engine. Il sera disponibles sur tous toutes les plateformes web.

## Comment joué :

Le joueur avance perpétuellement, il faut donc faire attention où l'on se dirige !

* Vise la direction avec la souris. 
* accélerer avec la barre espace
* Appuyer sur la touche P pour utiliser son pouvoir
<br/>

**Pour match a mort:**

* Donner un peu de nuage avec le click droit. 

<hr/>

Les nuages les plus petit se déplace plus rapidement que les gros.
Si un petit doit se diviser mais n'est pas assez gros -> meurt -> deviens des parcelles de nuages.

## But du jeux

Cloud_io a différents mode de jeux :

### 1. Mange les autres avant de te faire manger ! (inspiration : AGAR.IO)

Dans un monde limité deviens le plus gros nuage du ciel en mangeant les autres nuages plus petit. 
Plusieurs joueurs/nuages spawn en même temps aléatoirement dans la map, mais des joeurs peuvent rejoindre en pleine partie. Des parcelles de nuages sont placé un peu partout sur la map et le joueur peux le récupérer en passant dessus. 

Astuces :
* Attrapes un maximum de petit nuage au debut pour devenir de plus en plus gros !

Le joeur peut utiliser l'option boost :
* **Avantage** accélère la vitesse de déplacement par 1.5  
* **Inconvéniant** pendant l'utilisation du boost, la taille du nuage se réduit peu à peu

Pendant le boost une animation de pluie se produit.

Pour manger et corser les choses, des bonus et malus existent. 

#### Bonus

Avion freestyle :
Des petits avions se déplace rapidement dans la map (ils vont aussi vite que le boost) 
* Si le joueur arrive a le "manger", le joueur obtient un pouvoir de foudre qu'il peut utiliser sur les autres joueurs
**Propriété du bonus:**
Le joueur qui a la puissance chargé deviens un cumunolyngus et s'assombri, le temps chargé du bonus est limité.
Puissance chargé :
Le joueur peut utiliser son pouvoir sur 1 ou plusieurs énemies limités a sa vision. Lorsque celui-ci est touché il se split en 2 et il est immobilisé 2s (temps a définir).  


Convoit blindé :
Les convoits blindées sont un ensemble de 3 à 5 avions blindés qui se déplace dans la map. A endroit dans la map ils lacherons un convoit bonus en forme d'éclair. Un peu avant de lacher le convoit une croix se dessine sur la map, et tout les joueurs sont allerté. 

**Propriété du bonus:**
Lorsqu'un joueur récupère le bonus celui-ci grossi pendant un certaint temps (à définir) et peut accélerer en ilimité.

Peut être interrompue par :
* un nuage plus gros  
* Un avion blindé 
#### Malus

Avion blindé:
* Les avions blindés sont de gros avions qui se déplace en ligne droite et émettent une lumière rouge vers la direction à laquelle elle se déplace. A la différence avec les avions freestyle, les avions blindés ne peuvent pas être mangé, mais inflige des dégats (split en 2) si un joueur le touche. 

Chasseur :
Des avions très rapide se déplacant en sprirale. Si un joueur est touché par un chasseur il se splitera en 2.

Tornade :
Création d'un tourbillon qui attire les nuages entre eux -> les plus gros mangeront les plus petit. ⚠ La tornade en elle-même ne fais pas de dégats, elle ne fais que désorienté les joueurs !

* A définir -> la tornade split-il les gros nuages en 2 ?

**Apparition :**
* cas 1 :
    Une tornade peut spawn aléatoirement dans la map. Une indication alerte qu'une tornade approche.

* cas 2 :
    Apparation d'une tornade qui se déplace dans la map.
### 1.2 Avion freestyle

Au début de la partie le joueur à la possibilité de soit jouer les nuages, soit jouer les avions frestyle : 
L'avion fresstyle est un petit avion en bois. Le but est de 
faire un maximum de score acrobatique en un temps donnée sans ce faire manger par les joeurs nuages.

-> Définir point acrobatique 

Avec ses points ils pourront acheter des skins dans la boutique.

**Caractéristique de la map :**
* vide (pas d'intéraction)
* Limité en format carré
* Deplacement en X et Z
### 2. Survivre jusqu'au dernier

Un nombre de joueur est donnée en début de partie, et le but du jeux est d'être le dernier survivant.

![brouillon map](/preview/survive.JPG)

**Caractéristique de la map :**
* Une île avec une éolienne/ventillateur au centre de la map
* Limité format carré et se reduit avec le temps (zone)
* Deplacement en X ,Y et Z

Le principe reste le même, manger les autres sans te faire manger, mais il faut prendre en compte le ventillateur qui peut t'éjecter de la map. il faudra donc tourné autour de

Des parcelles de nuages sont placé un peu partout sur la map et le joueur peux le récupérer en passant dessus. Ces parcelles sont plus limité que dans le 1er mode de jeux. 

### 3. Labyrinthe, city

Ce mode de jeux permet d'intéragir avec la map. Le jeu ce déroule dans une ville de gratte-ciel. Et les joueurs doivent s'affronter à travers la ville. Si un joueur se prend un batiment, la partie qui touche le batiment se désagraige.

#### Piège dissimulé

Passage secret dans la map :
On peut se déplacer 

**Caractéristique de la map :**
* Limité format carré et se reduit avec le temps (zone)
* Deplacement en X ,Y et Z
### 4. Match a mort par équipe, chateau dans le ciel

Deux team s'affronte. L'équipe rouge et bleu.
But -> détruire le chateau adverse.

![brouillon map](/preview/match-a-mort-equipe.JPG)

2 façons de faires :
* Réduire le nombre de nuages sous les chateaux pour les faires tombées.
* Utiliser l'artefact au millieu (principe de la bombe atomique) pour assécher tout les nuages adverses.



**Choix du joueur :**
Nuage :
* Attaquant/ défenseur
Le but est de manger les autres nuages énemies, tout en protégant la base ou en la soigant.

**Capacité :**
Le joueur nuages a la possibilité de donner des parties de son nuages a la structure ou a d'autres nuages allié. 


Tourelle :
Les tourelles ont la capacité a ralentir les nuages énemies.
Pour les utilisés il faut que les joueurs nuages fassent un pont de nuages jusqu'a la tourelles. 

![brouillon map](/preview/equipe-tourelles.JPG)


⚠ Si le pont est brisé la tour ne fonctionnera plus.
⚠ Si un sort d'éclair est utilisé sur la tourelle, celle-ci est unitilisable pendant 8s (à définir)

**Bonbardier**
Les bombarbier sont des avions de voltige qui peuvent lancé une bombe a un endroit. C'est grâce au bombardier que l'on peut détruire le chateaux, une tourelle, ou encore un pont. 

Il est également possible d'attaquer un joueur nuage,mais les tirs de bombardier sont prévisble et lent (temps de décharge 2.5s) et seront donc facile a éviter (privililégiez les gros nuages ou les objets stationnaire). 

Un nuage a la possibilité de manger un bombardier. Si il y arrive il se transforme en cumunolingus et peut envoyé des éclairs au enemies.



### Coté estétique 

* caméra à la 3eme personnes en isométrique


A définir :

* La map -> s'éclairci en fonction du chemin parcouru ?
* Skins -> matériaux différent par rapport a des ref, peut-etre autre chose qu'un nuages.


### Bonus a définir

* Trompe oeuil (compact) :
Permet de faire croire au autre que l'on est plus petit que l'on est pendant un temps limité. 

* Mode Fantome -> arc en ciel:
On est invincible mais on ne peut manger personne, et les autres joeurs ne savent pas la taille que l'on a.

* Mode vergla (mode de jeux : XYZ):
fait tomber du vergla quand on se déplace.

