---
layout: post
title: "De la NP-complétude de l'allocation d'aiguilles"
---
L'objectif de notre projet est de générer des instructions à destination des tricoteurs, à partir d'un modèle donné en entrée. Pour parfaire ces instructions, indiquer le nombre d'aiguilles total à utiliser nous avait semblé une option intéressante ; restait simplement à trouver l'algorithme idéal pour calculer ce nombre, en le minimisant. Vous voyez venir d'ici les ennuis : le problème en question est NP-complet...
En effet, l'allocation des aiguilles est équivalente au problème de l'allocation de registres lors de la compilation d'un programme, ce dont on se rend compte en posant une analogie entre *splits* (séparation du tricot en deux branches au niveau d'un rang donné) et variables, et entre aiguilles et registres : le temps de vie d'une variable correspond à la longueur sur laquelle s'étend le *split*, et le registre dans lequel sera rangé cette variable correspond à l'aiguille supplémentaire qui permettra de tricoter la deuxième branche du *split*. 
En pratique, on peut raisonnablement imaginer que le nombre de *splits* sur une même pièce sera suffisamment faible pour que des algorithmes approchés suffisent à donner un nombre d'aiguilles, sinon minimal, du moins raisonnable.
