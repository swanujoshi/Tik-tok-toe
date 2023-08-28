# Tik-tok-toe
This repository contains a simple implementation of the classic Tic-Tac-Toe game using Python. The game is played in the command line interface and allows two players to take turns marking X and O on a 3x3 grid.The program checks for winning conditions, draws, and invalid moves, ensuring a smooth gaming experience 
You have a board list that represents the Tic-Tac-Toe game board. Each cell is initially marked with a "-".

The game starts with the "X" player.

The printBoard() function is used to display the current state of the game board.

The playerInput() function allows the human player ("X") to input their move. The input should be a number from 1 to 9, which corresponds to the positions on the board.

The checkHorizontle(), checkRow(), and checkDiag() functions check for horizontal, vertical, and diagonal wins respectively. If a win is detected, the corresponding player is declared the winner, and the game stops.

The checkIfWin() function checks for a win by calling the horizontal, row, and diagonal win checks.

The checkIfTie() function checks if the game has ended in a tie (i.e., all cells are filled).

The switchPlayer() function changes the current player from "X" to "O" and vice versa.

The computer() function simulates the computer's move. It selects a random empty position on the board and marks it with "O".

The main game loop runs as long as gameRunning is True. In each iteration, the board is displayed, the human player makes a move, win/tie conditions are checked, the player is switched, the computer makes a move, and win/tie conditions are checked again.

Overall, your code seems functional, but there are a few issues and improvements you could consider:

Typo: In the checkRow() function, where you set winner = board[3], it should be winner = board[2] instead.

Player Input Validation: You might want to add validation to ensure that the input from the human player is within the valid range (1-9) and corresponds to an empty cell on the board.

Computer Move Logic: The computer's move is currently made randomly. You could consider implementing a more sophisticated AI that tries to win if possible or blocks the human player from winning.

Function Organization: Consider organizing your code into classes and functions for better structure and readability.

Comments: Adding comments to explain each function's purpose and the overall game structure can make your code more understandable to others (and yourself) in the future.

Exit Condition: Currently, the game only stops when there's a win or a tie. You might want to provide an option for the player to exit the game before that point.

Remember, this is a basic implementation, and there are many ways to enhance and extend it.




