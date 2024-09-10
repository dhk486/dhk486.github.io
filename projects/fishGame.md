---
layout: project
type: project
image: img/fishGame.jpg
title: "Aloha Fish Master"
# All dates must be YYYY-MM-DD format!
date: 2024-09-09
published: true
labels:
  - Java
  - Group Progect
summary: "A text-based game I developed for ICS 211."
---

<img class="img-fluid" src="../img/fishGamePoster.png">

Aloha Fish Master is a Text-based Game for two players. The game is held for 12 months. Each player has 3 chances of catching fish in each month and they can use one of 5 methods: 'net', 'pole', 'spear', 'thow net', 'trap'.

To give you a flavor of the game, here is an excerpt from one run:

<hr>

<pre>
Code Information: 
  
  <img width="200px" src="../img/codeInfo.jpg">

  The picture above is a hierarchy of the Game. Describe the code briefly, 
  I_a is an abstract superclass for fall fish species. This is the backbone of all nethods which share with its subclass: Anae, Moi, Uhu, and Weke_a/Weke_ula.
  Fishable is Interface for I_a fish hierarchy.
  Anae, Moi, Uhu, Weke_a/ Weke_ula are subclasses creating each fish data.
  FishDriver is the driver class for the game. To prevent poor readability, Inpur codes and output codes are created as independent classes then instantiated in FishDriver class. 

  Visual of Game:
  When one player starts the game, they would see menu like below:

  <img width="200px" src="../img/visual1.jpg">

  Then The player can choose a method to catch fish.

  <img width="200px" src="../img/visual2.jpg">

  Information of fish they caught is shown on the screen and they will be asked to see rules about fishing. Some fish has legal minimum size that players allow to catch. If a player put into illegal size of fish into their sack, all of fish they have catched would be confiscated. Players always see the legality on the menu.

  <img width="200px" src="../img/visual3.jpg">

  Once 12 months of turns are taken, the player whose sum of the 3 largest fish' lengths is greater will be the winner of the game.

  <img width="200px" src="../img/visual4.jpg">
  
</pre>

<hr>

Source: 
