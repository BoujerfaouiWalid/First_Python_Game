
## Tic-Tac-Toe Game in Python

This is a Tic-Tac-Toe game built using Python's tkinter library, which provides a graphical user interface (GUI). The game supports two modes: Player vs. Player (PvP) and Player vs. Computer (PvC), allowing you to play against another human or the computer.

## Features
# Graphical Interface:
The game has a 3x3 grid where players can take turns to place their marks.
# Player vs. Player Mode: 
Two players can compete against each other, with the interface alternating between players 'X' and 'O'.
# Player vs. Computer Mode: 
Play against a simple AI where the computer randomly selects empty spaces on the grid.
# Win Detection: 
The game automatically detects when a player wins or if the game ends in a draw.
# Reset Option: 
After each game, players can reset the board to play again.
## How the Game Works
Game Modes
# Player vs. Player (PvP):

Two players alternate turns by clicking on the grid cells. Player 'X' always goes first.
The first player to get three of their marks (either 'X' or 'O') in a row (horizontally, vertically, or diagonally) wins the game.
If all the cells are filled and no player has won, the game ends in a draw.

# Player vs. Computer (PvC):

In this mode, Player 'X' is controlled by a human, and Player 'O' is controlled by the computer.
The computer makes random moves on its turn.
The win conditions are the same as in the PvP mode.

# Winning Conditions
A player wins if they manage to place three of their marks ('X' or 'O') in:
A horizontal line
A vertical line
A diagonal line
Resetting the Game
The game provides a Reset Game button that clears the board, resets the turn to Player 'X', and allows players to start a new round.

## Code Overview

The game is implemented in the TicTacToeApp class, which uses tkinter to build the GUI.

- __init__(self, root): Initializes the game, sets up the board, and displays the current player's turn.
- create_widgets(self): Creates the GUI layout, including buttons for the grid, mode selection, and reset.
- on_button_click(self, row, col): Handles the player's move when they click on a grid cell.
- check_winner(self): Checks if there is a winner after every move.
- is_board_full(self): Checks if the board is full, leading to a draw.
- computer_move(self): Handles the computer's move by randomly selecting an empty cell.

## Installation

# Clone the repository:
git clone https://github.com/yourusername/tic-tac-toe.git

# Navigate to the project directory:
cd tic-tac-toe

# Run the game:
python tictactoe.py

# !!! Make sure you have Python installed. This game requires no additional dependencies beyond the standard tkinter library, which comes with most Python installations.


