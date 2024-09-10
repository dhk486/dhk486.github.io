---
layout: project
type: project
image: img/hangman.png
title: "Hangman Game"
# All dates must be YYYY-MM-DD format!
date: 2024-09-09
published: true
labels:
  - C
  - Game
summary: "A Simple world-guessing game."
---

<img class="img-fluid" src="../img/hangman_header.png">

This is a Hangman Game, a simple word-guessing game where the player tries to guess a hidden word letter by letter. The player has a limited number of incorrect guesses before losing the game. This game is created with array, loop operations, and if statements. 

This game was created to practice making an array, loop operations and if statements. 
<hr>
When the player starts the game, a random word is chosen from a predefined list of array called 'words' using rand().

The player can see the word, with each letter hidden as an underscore.

<img width="200px" src="../img/hangman.png" >

The player guesses letters, and if the letter that the player entered exists in the word, it is revealed in the correct position. 

<img width="200px" src="../img/correct.png" >

If the player guesses wrong, the visual representation of a stick figure on a gallows (the "hangman") progress.

<img width="200px" src="../img/incorrect.png" >

The game ends when the player either guesses the word correctly or reaches 6 wrong guesses. 

<img width="200px" src="../img/endOfGameFail.png" >
<img width="200px" src="../img/endOfGameWin.png" >

</pre>

<hr>

Source:
