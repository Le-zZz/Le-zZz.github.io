# Dungeon Survivor

## Introduction

Dans le cadre d'un projet scolaire visant à nous évaluer sur l'implémentation d'une génération procédurale et d'une intelligence artificielle, le jeu dungeon survivor est née.
Dungeon Survivor est shooter2D vu du dessus ou l'on doit survivre a l'attaque des different zombies, tout en recoltant des items pour pouvoir survivre
Pour la création de celui-ci, j'ai fais équipe avec l'une de mes camarades de classe, Solange.

## Présentation:

On incarne un humain armé d'un pistolet qui se trouve dans un salle avec une horloge et le but est de parcourir un dongeon rempli de zombies afin de trouver une clé permettant d'ouvrir l'horloge et pouvoir s'échapper. 

Pour commencer, nous avons partager les tâches. J'étais chargé des 3C (caméra, control, character), de la génération procédurale, IA. Solange était chargé des ennemis, level design, des animations, des sons, des menus. On a travaillé en équipe et on s'est aidé du mieux qu'on pouvait.0


## 3C :

En ce qui concerne le joueur, il peut se déplacer et tirer et il peut se faire attaquer et ainsi perdre de la vie. Il se déplace avec les touches WASD et sa rotation suit la position de la souris. Pour tirer, il faut appuyé sur le clique gauche.
La caméra suit en permanence le joueur.

## Ennemy : 


## Generation Procédurale :

En ce qui concerne la génération procédurale, on a opté pour un système de salle pré-fabriqué. Chaque salle possède plusieurs points de spawn pour les ennemies et les objects de soins qui sont générés en même temps.

## IA :

Toutes les salles ont une formee rectangulaire et excepté la salle de départ qui possède 4 sorties ouvertee, les autres salles possèdent entre 1 ou 2 sorties ouvertes.
Arrivé à 10 salles généré, la probabilité qu'une salle à une sortie puisse être généré augmente et ainsi provoqué la fin de la génération procédurale et boucler la map.


## Conclusion :
