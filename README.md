# TicTacToe AI
A TicTacToe decision-based AI written in Python to demonstrate the minimax algorithm for turn-based games.

TicTacToe is a solved game with a relatively small finite set of possible games. A graphical map of optimal TicTacToe moves can be found at https://xkcd.com/832/. Knowing the optimal move for any game state makes it possible to write an ideal TicTacToe AI using a lookup table. But where's the fun in that?

This AI searches a pruned subset of the game tree starting from the given game state to find the best possible move using minimax decision making. We can evaluate the effectiveness of this AI by comparing its decisions to the optimal moves from the ideal lookup table.

## The Minimax Algorithm
[Minimax](https://en.wikipedia.org/wiki/Minimax) is a decision rule originally formulated for two-player zero-sum game theory for minimizing one's own maximum loss which is identical to minimizing the opponent's maximum payoff. The player assigns values to the outcomes of a game and selects the option leading to the maximum outcome by working backwards from the end of the game knowing that the opponent will always select the minimal option on their turn.

#How to Run
- Running texttictactoe.py provides a command line interface for playing the game against the AI opponent. The player enters their move by submitting a row number then submitting a column number.
- Running tictactoe.py has the AI play against itself in the command line.

The board is modeled as a 2D string array. Example below:

```
board = [
    ["X", " " ,"O"], 
    [" ", "O" ," "], 
    ["X", " " ,"X"]
]
```
