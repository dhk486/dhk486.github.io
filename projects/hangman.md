---
layout: project
type: project
image: img/hangman-square.png
title: "Hangman Game"
# All dates must be YYYY-MM-DD format!
date: 2024-09-09
published: true
labels:
  - C
  - Console Game
  - Game Development
  - Random Word Generation
summary: "A Simple world-guessing game."
---

<img class="img-fluid" src="../img/hangman_header.png">

## Project Description

The Hangman game is a classic word-guessing game implemented in C. This console-based version challenges players to guess a hidden word by suggesting letters within a limited number of incorrect guesses. The game features a visual representation of the hangman that progresses with each incorrect guess, adding a fun and interactive element to the gameplay.

This game was created to practice making an array, loop operations and if statements. 

<hr>

## Features

* Word Selection :
  The game randomly selects a word  from a predefined list of 25 words, including various animals such as "dog," "cat," and "tiger."
* Gameplay Mechanics:
  Players guess letters to reveal parts of the hidden word. Correct guesses show the letter in its correct position, while incorrect guesses increase the number of mistakes.
* Hangman Drawing:
  **score() function displays a hangman graphic that evolves with each incorrect guess, providing visual feedback on the player's performance.

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
