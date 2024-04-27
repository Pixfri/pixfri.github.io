---
title: "Les Blocks et les BlockStates dans Minecraft"
date: "2023-09-27T19:57:00+02:00"
author: "Jean Letessier"
description: "Que sont les blocks et les blockstates dans Minecraft ? Comment sont-ils utilisés ? Quelles sont les différences entre les deux ?"
draft: false
aliases: [
    "blockstates"
]
tags: [ 
  "Resource Packs",
  "Modding",
  "Minecraft"
]
autonumber: true
---

## Plan de l'article
1. [Qu'est-ce qu'un block ?](#quest-ce-quun-block-)  
2. [Qu'est-ce qu'un blockstate ?](#quest-ce-quun-blockstate-)  
3. [Conclusion](#conclusion)

## Qu'est-ce qu'un block ?

Beaucoup de gens définissent les blocs dans minecraft comme les cubes qui composent le monde, mais ce n'est pas tout à fait vrai.
En effet, un Block, du côté du code source du jeu, ne sert que de patron pour définir le comportement d'un bloc. Il ne contient pas
de données sur l'état du bloc, ni sur son emplacement dans le monde. Les blocs ne sont enregistrés qu'au lancement du jeu.

## Qu'est-ce qu'un blockstate ?

Un `blockstate` lui est une représentation du bloc dans le monde, il contient des données sur l'état du bloc (comme
son emplacement dans le monde, sa rotation, ou même certaines propriétés, si une lampe en redstone est allumée par exemple). 
Ce sont eux que nous voyons dans le monde. Les blockstates eux, sont créés et sauvegardés dans les chunks.

Ces blockstates permettent de changer le comportement de bloc ainsi que son modèle en fonction de ses propriétés. Par exemple,
un escalier va changer de modèle en fonction de son orientation, de s'il est en haut ou en bas d'un bloc, si un autre escalier
dans une autre orientation est à côté de lui, etc.

Le modèle que le bloc va prendre en fonction des propriétés des blockstates est défini dans un fichier json, se trouvant dans
le dossier `assets/minecraft/blockstates/<nom_du_bloc>.json` du resource pack que vous utilisez. Ce fichier contient une liste de variantes, qui représentent
quel modèle charger en fonction des propriétés.

*À noter que le `minecraft` peut être remplacé par l'id de votre mod.

## Conclusion

Pour résumer, un block est le patron, la représentation de votre block et de son fonctionnement dans le code du jeu, 
tandis qu'un blockstate est la représentation de votre block dans un état précis à l'intérieur du monde.

Voici la fin de cet article assez court sur la différence entre un block et un blockstate. J'espère vous avoir appris 
quelque chose sur le fonctionnement du jeu. 
