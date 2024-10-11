Tic-Tac-Toe Game in C++
Overview
Welcome to the Tic-Tac-Toe game! This project is a fun and interactive command-line version of the classic Tic-Tac-Toe game, allowing players to challenge an intelligent AI opponent. The AI is powered by the Minimax algorithm, ensuring it plays optimally and provides a competitive gaming experience.

Table of Contents
Features
Gameplay Instructions
Running the Game
Code Structure
License
Features
Engaging Gameplay: Play against a smart AI that never loses, thanks to the Minimax algorithm.
User-Friendly Interface: Simple command-line interface for easy interaction.
Dynamic Game State Management: Detects wins, draws, and invalid moves in real-time.
Optimized AI Strategy: The AI employs a robust strategy to provide challenging gameplay.
Gameplay Instructions
How to Play
Game Setup: A 3x3 grid is presented with slots numbered 1 through 9.
Player Symbols: You will play as X, while the AI will be O.
Making Your Move: You start the game by choosing a number (1-9) that corresponds to the desired position on the grid.
AI's Turn: After your move, the AI will calculate and make its move.
Game Continuation: The game continues until either you or the AI wins, or the game results in a draw.
Example Gameplay
plaintext
Copy code
 1 | 2 | 3
---|---|---
 4 | 5 | 6
---|---|---
 7 | 8 | 9

Player X, enter your move (1-9): 5
AI (O) moves to slot 1

 O | 2 | 3
---|---|---
 4 | X | 6
---|---|---
 7 | 8 | 9
Winning Conditions
Winning the Game: Align three of your symbols (X or O) in a row, column, or diagonal.
Draw Condition: The game ends in a draw if all slots are filled without a winner.
Running the Game
Prerequisites
A C++ compiler (e.g., g++, clang) installed on your machine.
Compilation Instructions
To compile the game, use the following command:

bash
Copy code
g++ -o tictactoe tictactoe.cpp
Starting the Game
To start the game after compilation, run:

bash
Copy code
./tictactoe
Code Structure
Main Functions
initializeBoard(): Sets up the initial game board with numbered slots.
printBoard(): Displays the current layout of the board.
isMovesLeft(): Checks for any remaining moves on the board.
evaluateBoard(player, opponent): Assesses the board to determine if there's a winner.
minimax(currentPlayer, ai, human, isMaximizing): Implements the Minimax algorithm to find the optimal move for the AI.
findBestMove(ai, human): Identifies the best move available for the AI.
placeMarker(slot, marker): Places the player's marker in the chosen slot.
checkWin(marker): Checks if the specified marker has won the game.
checkDraw(): Determines if the game has ended in a draw.
License
This project is open-source and is licensed under the MIT License.

