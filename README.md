# Dungeon Survivor

## Introduction

Dans le cadre d'un projet scolaire visant à nous évaluer sur l'implémentation d'une génération procédurale et d'une intelligence artificielle, le jeu Dungeon Survivor est née.
Dungeon Survivor est shooter 2D vu du dessus où l'on doit survivre à l'attaque des différents zombies, le but étant de rejoindre la salle du coffre pour gagner.
Pour la création de celui-ci, j'ai fais équipe avec l'une de mes camarades de classe, Solange.

## Generation Procédurale :

![map](zCallMeZ.github.io/assets/gif/map.gif)

En ce qui concerne la génération procédurale, on a opté pour un système de salles pré-fabriqué dans un espace de 4 sur 4. La première salle spawn et haut de la grille et à partir de ce moment, elles peuvent spawner et se dirigier dans 3 direction. A gauche, à droite ou en bas. 

Sortie gauche et droite :
![LR](zCallMeZ.github.io/assets/gif/LR.JPG)
Sortie gauche, droite et haut:
![LRB](zCallMeZ.github.io/assets/gif/LRB.JPG)
Sortie gauche, droite et bas : 
![LRT](zCallMeZ.github.io/assets/gif/LRT.JPG)
Sortie gauche, droite, bas et haut :
![LRBT](zCallMeZ.github.io/assets/gif/LRBT.JPG)

Ensuite lors du lancement du script dans la fonction Start, on determine 
![Start](zCallMeZ.github.io/assets/gif/Start.JPG)
![update](zCallMeZ.github.io/assets/gif/update.JPG)
![spawnennemy](zCallMeZ.github.io/assets/gif/spawnennemy.JPG)

![direction1](zCallMeZ.github.io/assets/gif/direction1.JPG)
![direction3](zCallMeZ.github.io/assets/gif/direction3.JPG)
![direction5](zCallMeZ.github.io/assets/gif/direction5.JPG)
![stopgen true](zCallMeZ.github.io/assets/gif/stopgen true.JPG)
