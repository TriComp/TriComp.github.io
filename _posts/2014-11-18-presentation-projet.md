---
layout: post
title: "Présentation du projet"
---
Le projet TriComp a été réalisé dans le cadre de notre M1 d'informatique à l'ENS de Lyon.

Notre objectif est de produire un assistant de tricot, permettant d'une part de décrire des pièces de tricot (écharpes, pulls, housses de fauteuils...), et d'autre 
part, à partir de cette description, de générer une suite d'instructions (à destination du tricoteur) permettant de confectionner la pièce en question.

La description "source" des pièces de tricot, si elle peut se faire *via* une interface graphique, est stockée sous la forme d'un programme dans un langage défini 
pour l'occasion (et peut d'ailleurs directement être définie sous cette forme). L'un des enjeux du projet est donc de transformer cette description "haut niveau" de 
l'objet en une description "bas niveau" (la suite des mailles à tricoter pour la réaliser) : c'est pour cela qu'il avait initialement été pensé comme un 
"compilateur de tricot", d'où son nom.

Le projet en lui-même est composé de plusieurs modules : 
* l'interface graphique
* la définition et la spécification des langages bas et haut niveau
* le compilateur (parsage du langage de haut niveau et conversion en langage de bas niveau)