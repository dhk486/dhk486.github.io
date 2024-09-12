---
layout: project
type: project
image: img/fishGame-square.jpg
title: "Aloha Fish Master"
# All dates must be YYYY-MM-DD format!
date: 2024-09-09
published: true
labels:
  - Java
  - Group Progect
  - Object Hierarchy
  - Text-Based Game
summary: "A text-based game I developed with group memembers for ICS 211."
---

<img class="img-fluid" src="../img/fishGamePoster.png">

## Project Summary

This **_Aloha Fish Master_** is a group project assignment when I was taking ICS 211 at Kapiolani Community College in Fall 2023. Each member is supposed to complete an Object Oriented Class hierarchy modeling Hawaiian Fish famillies. In this project, we have the given **_I_a abstract super class_** and implemented three fish types: **_'Ama'ama Family, Weke Family, Uhu Family_**. Then, we built a 2 players text-baded fishing tournament game program using **_I_a object classes_**. My task was implementing **_Uhu Family_** which has **_Ohua Class_**, **_Panuhunuhu Class_**, **_Uhu Class_**. Also, I designed the poster of our project. 

<hr>

## Brief Information of the Project

Aloha Fish Master is a Text-based Game for two players. The game is held for 12 months. Each player has 3 chances of catching fish in each month and they can use one of 5 methods: 'net', 'pole', 'spear', 'thow net', 'trap'.

To give you a flavor of the game, here is an excerpt from one run:

<hr>

## Code Information: 
  
  <img width="600px" src="../img/codeInfo.jpg">

  The picture above is a hierarchy of the Game. Describe the code briefly, 
  I_a is an abstract superclass for fall fish species. This is the backbone of all nethods which share with its subclass: Anae, Moi, Uhu, and Weke_a/Weke_ula.
  Fishable is Interface for I_a fish hierarchy.
  Anae, Moi, Uhu, Weke_a/ Weke_ula are subclasses creating each fish data.
  FishDriver is the driver class for the game. To prevent poor readability, Inpur codes and output codes are created as independent classes then instantiated in FishDriver class. 

<hr>

## Visual of Game:

  When one player starts the game, they would see menu like below:

  <img width="600px" src="../img/visual1.jpg">

  Then The player can choose a method to catch fish.

  <img width="600px" src="../img/visual2.jpg">

  Information of fish they caught is shown on the screen and they will be asked to see rules about fishing. Some fish has legal minimum size that players allow to catch. If a player put into illegal size of fish into their sack, all of fish they have catched would be confiscated. Players always see the legality on the menu.

  <img width="600px" src="../img/visual3.jpg">

  Once 12 months of turns are taken, the player whose sum of the 3 largest fish' lengths is greater will be the winner of the game.

  <img width="600px" src="../img/visual4.jpg">

<hr>

  
</pre>

<hr>

Source: 
