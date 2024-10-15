# Hangman Game - README

## Overview
This is a simple console-based Hangman game implemented in Python. The player tries to guess a randomly selected word by guessing one letter at a time. The player has a limited number of incorrect guesses before losing the game.

## Features
- Random word selection from a predefined list.
- ASCII art representation of the Hangman for each incorrect guess.
- Tracks and displays guessed letters.
- User-friendly prompts and feedback.

## Code Breakdown

### Functions

- **get_random_word()**
  - Returns a random word from a list of programming-related terms (e.g., `['python', 'java', 'html', 'sql']`).

- **display_hangman(tries)**
  - Takes the number of incorrect tries as an argument and returns the corresponding Hangman ASCII art stage.
  - There are four stages: fully hanging, torso, head, and empty gallows.

- **play()**
  - The main function that drives the game:
    - Initializes game variables: `word`, `word_letters`, `guessed_letters`, and `tries`.
    - Displays the welcome message.
    - Runs a loop that continues until the player either guesses the word or runs out of tries:
      - Displays the current Hangman stage, guessed letters, and the word with unguessed letters represented as underscores.
      - Prompts the player for a letter guess and checks its validity.
      - Updates the game state based on the player's guess.

## Main Execution Block
- Calls the `play()` function if the script is run as the main program.

## Usage
1. Ensure you have Python installed on your machine.
2. Copy the code into a `.py` file (e.g., `hangman.py`).
3. Run the script in a terminal or command prompt using:
   ```bash
   python hangman.py
