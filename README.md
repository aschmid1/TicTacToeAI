# TicTacToe AI
A TicTacToe AI written in Python with minimal lookup tables to demonstrate a min-max search algorithm for turn-based games.

TicTacToe is a solved game with a relatively small set of possible games making it reasonable to write an AI using a lookup table. This also gives us an easy way to evaluate the effectiveness of a TicTacToe AI by comparing its moves to the optimal moves from the lookup table. A graphical map of optimal TicTacToe moves can be found at https://xkcd.com/832/ for an idea of what the lookup table would contain.

#Board Model and UI
The board is modeled as a 2D string array. An example is shown below:

```
board = [
    ["X", " " ,"O"], 
    [" ", "O" ," "], 
    ["X", " " ,"X"]
]
```

Running texttictactoe.py provides a command line interface for playing the game against the AI opponent.