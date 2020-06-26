# Dungeon Survivor

## Introduction

Dans le cadre d'un projet scolaire visant à nous évaluer sur l'implémentation d'une génération procédurale et d'une intelligence artificielle, le jeu Dungeon Survivor est née.
Dungeon Survivor est shooter 2D vu du dessus où l'on doit survivre à l'attaque des différents zombies, tout en récoltant des items pour pouvoir survivre.
Pour la création de celui-ci, j'ai fais équipe avec l'une de mes camarades de classe, Solange.

![examples](zCallMeZ.github.io/assets/gif/examples.png)

## Présentation:

On incarne un humain armé d'un pistolet qui se trouve dans une salle avec une horloge et le but est de parcourir un dongeon rempli de zombies afin de trouver une clé permettant d'ouvrir l'horloge et pouvoir s'échapper. 

Pour commencer, nous avons partager les tâches. J'étais chargé des 3C (caméra, control, character), de la génération procédurale, IA. Solange était chargé des ennemis, level design, des animations, des sons, des menus. On a travaillé en équipe et on s'est aidé du mieux qu'on pouvait.


## 3C :

En ce qui concerne le joueur, il peut se déplacer et tirer et il peut se faire attaquer et ainsi perdre de la vie. Il se déplace avec les touches WASD et sa rotation suit la position de la souris. Pour tirer, il faut appuyé sur le clique gauche.
La caméra suit en permanence le joueur.

## Ennemies : 

En ce qui concerne les ennemies, on a décidé d'intégrer 3 types de zombies.

Le premier se nomme "Zombie Classique", il a un comportement qu'on peut retrouver dans la majorité des jeux de zombies. Il réagit et attaque dès que le joueur se trouve dans son champ de vision. Tout ceci marche à l'aide de Transform et de Trigger. 

Le deuxième se nomme "Zombie Kamikaze", il attaque le joueur dès qu'il est à ça porter et il explose au contact de celui-ci, ce qui cause de gros dégâts. Tout ceci marche à l'aide de Transform et de Trigger. 

Le dernier se nomme "Zombie Tank", il se déplace autour des coffres qui contiennent les clés qui permettent d'activer l'horloge pour s'évader du donjon et ainsi compléter le jeu et possède un nombre de point de vie assez élévé. Sa particularité est qu'au contact du joueur, celui-ci perd de la vie et est directement téléporter au début du niveau. Tout ceci marche à l'aide de Transform et de Trigger.

## Generation Procédurale :

En ce qui concerne la génération procédurale, on a opté pour un système de salle pré-fabriqué. Chaque salle possède plusieurs points de spawn pour les ennemies et les objects de soins qui sont générés en même temps. 

Le processus se déroule de la manière suivante :

-Toutes les salles ont une formee rectangulaire sauf la salle de départ qui possède 4 sorties ouvertee, les autres salles possèdent entre 1 ou 2 sorties ouvertes.

-Chaque salle vérifie si dans chacune de ses directions, il y a déjà une salle et si ce n'est pas le cas, Elle en génère une. Ensuite, une fois que cette salle est génère, elle regarde dans quelle direction elle peut y aller, et s'il n'y a pas de salle dans la direction dans laquelle est peut y aller, elle en génère une. Et ainsi de suite.

-Dès que 10 salles sont générées, la probabilité qu'une salle à une sortie puisse être généré augmente et ainsi provoqué la fin de la génération procédurale et boucler la map.

## IA :

En ce qui concerne l'intelligence artificielle, nous avons crée un script avec un système de pathfinding avec la méthode A* assez connu dans le milieu. Elle consiste a évolué le "coût" de déplacement d'un ennemi afin d'opter pour le chemin le moins chère pour atteindre son objectif. Les déplacements horizontale et verticale son les moins chères, les diagonales sont plus éléves et passer à travers un mur est impossible. 

Tout ces déplacement fonctionnent grâce aux différents points générés au même moment que la map.

Malheuresement, on n'a pas reussit à l'implémenter correctement dans notre jeu par manque de temps et de compréhension.

Nous avons rencontrer des problèmes aux moments de lier la TileMap et les waypoints avec nos scripts de génération de map et joindre les deux nous a été impossible.

## Conclusion :

Pour conclure, d'un point de vue purement personnel, cela a été un déssastre. Que ce soit de mon côté ou celui de ma partenaire, beaucoup d'obstacles se sont présentés à nous, que ce soit dans la vie privée, vie professionnel ou tout simplement celle d'un simple étudiant.

Pour ma part, je me suis jamais considéré comme quelqu'un qui avait des facilitées avec la programmation et ce projet n'a fait que reforcer mes propos. Le manque de temps à cause du travail ne m'a pas facilité la tâches. 
Je travaille de jeudi à mardi 9h par jour et le reste le temps je le passe à l'école ou à étudier. 

Ce qui m'a manqué pour pouvoir finaliser ce projet comme je l'aurais voulu était plus de temps pour pouvoir apprendre et comprendre mieux le fonctionnement de tel ou tel implémentation et comprendre la logique qu'il y a derrière.

Ce que ce projet m'a apporté est de meilleur connaissance dans la programmation, une meilleure autonomie, une méthode de travail plus strict, une capacité de travail en équipe acrue et une motivation à me donner à 1000% pour continuer mes études, car tous ses sacrifices que je fais pour pouvoir rentrer dans l'industrie à l'avenir ne fait que croître.
