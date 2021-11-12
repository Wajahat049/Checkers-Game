# CHECKERS GAME

<img src="https://user-images.githubusercontent.com/64039135/141333431-69cf12e8-a40d-4163-bccc-9372ef82f043.PNG" width="500px" height="400px" />

## INTRODUCTION
Checkers is a group of strategy board game is played by two opponents, on opposite sides of the game board. One player has the dark pieces; the other has the light pieces. At the start of the game, each contestant has 12 pieces arranged on the board.

## RULES:
Players have alternate turns. A move consists of moving a piece diagonally to an adjacent unoccupied square. If the adjacent square contains an opponent's piece, and the square immediately beyond it is vacant, the piece may be captured by jumping over it and that piece is removed from the game. When a piece first enters the opponent’s last back row and it is crowned. The piece, now called a king, has the added privilege of moving and jumping backward.
In almost all variants, the player without pieces remaining, or who cannot move due to being blocked, loses the game.

## PYGAME:
Pygame is a free and open-source cross-platform library for the development of multimedia applications like video games using Python.
This Checker is implemented by using Pygame.

## HOW IT WORKS:
Black Pieces are moved by players and White pieces are automatically moved by computer. An Algorithm known as minimax is implemented by which computer plays against the player.
If a player clicks on his piece the computer also shows the hint by a red spot and player can choose the place as where to move his piece.
The Player and computer can dismiss each other pieces by jumping upon them.
If all the Black pieces are gone first, then White wins and if all the White pieces are gone first, then Black wins.

## VALID MOVES ALGORITHM:
An Algorithm to get all the valid moves.
1. First a dictionary of moves is initialized then we implement condition to check out the color of the piece.
2. If the color of our piece is Black then we use traverse left or traverse right function to move our piece up the board traverse_left or traverse_right functions also check when and where to jump upon an opponent’s piece, when to double jump or triple jump.
3. These functions are defined so that they make best possible move.
4. In the same way, If the color of our piece is White then we uses traverse_left or traverse_right function to go down the board.

## MINIMAX ALGORITHM:
An Algorithm to check which piece to move so that we get best results
1. Computer (White piece) is a maximizing player and the player (Black piece) is a minimizing one.
2. best_move variable holds a reference to a Move object.
3. A condition to check whether the player is max_player or min_player is implemented.
4. In case of max_player maxEval is initialized to negative infinity (-∞) .
5.  Otherwise, minEval is initialized to positive infinity (-∞).
6. Now we run minimax function recursively to a certain depth to check for all the possible moves.
7. Now a deep copy of the whole board is made.
8. All the set of moves are applied on the board to check which set of moves would get max score.
9. Then the set of moves giving best possible score by moving a piece is applied on real board.


For just an idea that how the minimax algorithm works there is a tree in which you can see that on the last level we take the max of set the scores then on 3rd level we take min of set of scores and this alternation continues till we reach the root and then on the root we take max of the scores.

<img src="https://user-images.githubusercontent.com/64039135/141335513-5205acc0-f00b-45a3-bb1c-05448df32df8.PNG" width="700px" height="400px" />
