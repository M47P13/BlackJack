# Blackjack Game Documentation

## Introduction

This document provides an overview of a simple Blackjack game implemented using HTML, CSS, and JavaScript.

## HTML Structure

The game interface is created using HTML and consists of the following elements:

- `<h2>` elements to display the dealer's and player's current sums.
- `<div>` elements to display the dealer's and player's cards.
- "Hit" and "Stay" buttons to interact with the game.
- A paragraph element to display the game results.

## JavaScript Functions

### `buildDeck()`

This function initializes an array called `deck`, which represents a standard deck of 52 playing cards. It combines card values ("A" to "K") and card types ("C" for Clubs, "D" for Diamonds, "H" for Hearts, and "S" for Spades) to create card names like "A-C" for Ace of Clubs.

### `shuffleDeck()`

This function shuffles the `deck` array by randomly swapping card positions. It uses a Fisher-Yates shuffle algorithm to ensure randomness.

### `startGame()`

This function starts the game by initializing the dealer's and player's hands. It also sets up event listeners for the "Hit" and "Stay" buttons.

- The dealer receives one face-down card (`hidden`) and one face-up card.
- The player receives two face-up cards.
- The dealer's logic is automated to draw cards until their sum is at least 17.

### `hit()`

This function is called when the player clicks the "Hit" button. It allows the player to draw one card from the deck and adds it to their hand. The function checks for the value of Aces to prevent the player from going over 21.

### `stay()`

This function is called when the player clicks the "Stay" button. It calculates the final scores for both the dealer and the player, taking into account the value of Aces. Then, it determines the game outcome and displays a message.

### `getValue(card)`

This function extracts the numeric value of a card. Face cards (J, Q, K) are assigned a value of 10, and Aces are initially assigned a value of 11.

### `checkAce(card)`

This function checks if a card is an Ace and returns 1 if true, or 0 if false.

### `reduceAce(playerSum, playerAceCount)`

This function reduces the value of Aces from the player's sum to prevent them from busting (going over 21) if necessary.

## Usage

To play the game:

1. Open the HTML file in a web browser.
2. Click the "Hit" button to draw cards.
3. Click the "Stay" button to end your turn.
4. The game will determine the winner and display the result.

## Conclusion

This simple Blackjack game allows you to play against a computer dealer. It includes basic game logic, card handling, and scoring. You can customize and expand upon this code to create a more complex Blackjack game.

# Project Overview

I have developed a simple Blackjack game in JavaScript and HTML. This project serves as a learning exercise to enhance my skills as a software engineer. The game allows players to compete against a computer dealer, with the goal of getting as close to 21 as possible without exceeding it. 

## Purpose

The purpose of creating this software is to:

1. **Improve JavaScript Skills:** This project provides an opportunity to practice and improve my JavaScript programming skills, event handling, and logic implementation.

2. **Interactive Web Development:** It allows me to create an interactive web application. Understanding how to create user interfaces and handle user interactions is crucial.

3. **Problem Solving:** Developing a game like Blackjack involves solving complex problems related to card handling, scoring, and game logic. It's a great way to enhance problem-solving skills.

## Software Demo

You can watch a brief one-minute demonstration of the software in action by following the link below:

[Software Demo Video](https://youtu.be/ApGzNkO1b3Q)

# Development Environment

I used the following tools and technologies to develop this software:

- **HTML:** The game's user interface is built using HTML, which provides the structure of the web page.

- **CSS:**  CSS is used for styling and layout.

- **JavaScript:** The core functionality of the game is implemented in JavaScript. This includes shuffling the deck, handling card values, managing player and dealer hands, and determining the game's outcome.

- **Code Editor:** I used a code editor - Visual Studio Code to write and debug the code.

- **Web Browser:** To test and run the game, I used a web browser (Chrome, Firefox, or Edge).

- **YouTube:** I used YouTube to host and share the demo video of the software in action.

By working on this project, I aimed to gain practical experience in web development and JavaScript programming, as well as to demonstrate my ability to create interactive and engaging web applications.

# Useful Websites

{Make a list of websites that you found helpful in this project}
* [W3 Tutorials](https://www.w3schools.com/js/js_intro.asp)
* [Blackjack](https://math.hws.edu/eck/cs271/js-work/Blackjack.html)