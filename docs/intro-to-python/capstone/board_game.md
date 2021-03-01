---
title: Application - 🎲 Board games
date: 06/02/2021
mentors: 
  - TimSando
tags:
  - Emulation
  - Board Game
links:
  - '[Capstone template code](https://github.com/CapgeminiInventIDE/PyCap/tree/main/src/intro-to-python/capstone/board_game){target=_blank}'
---

{{ course_summary(title, date, mentors=mentors, tags=tags, links=links) }}

## Problem

Create a basic commandline application using Python 3.6+ that allows a user to play a game of "pythons" and ladders (snakes and ladders).
Your code should be well documented with a docstrings, comments and a README describing how your program works, unit tests to ensure it works as expected and type annotations and finally well formatted using Black. This is so other developers can understand how to help build upon your program.

You should add a summary to your README that includes the next steps (dot points) and also the strengths and weaknesses of your program in its current state.
A list of operations that your should support, as well as how we expect them to be called can be found in the table below.

> Each board should be composed of a 5x5 grid where each square can either be blank, a python or a ladder. If it is a python or a ladder, then we need to know what square it leads to.

| Operation                                            | Usage |
|------------------------------------------------------|-------|
| Start a new single player game                      | `"python board_game.py"`      |
| Keep the game running until cancelled by the player  | `"Game is active"`      |
| Roll a 6 sided die                                | `"Press a button to roll the die"`      |
| Print out the player's current location on the board | `"Press a button to show current location"`      |
| Move a player to a new square based on their die roll | `"Moving player forward x squares"`      |
| Move a player to a different square if it lands on a python  | `"Player landed on a python, sliding back to square X"`      |
| Move a player to a different square if it lands on a ladder  | `"Player landed on a ladder, climbing up to square X"`       |
| Game finishes when the player exceeds the final square | `"You've reached the final square and won the game. Congratulations!"`      |

## Optional Extras

- Dynamically generate a new board each game using code
- Make a the game multiplayer
- Visualise the board layout
- Require the final roll to be the exact number required to get to 25 or else move back squares
- Save a game in progress and load it later