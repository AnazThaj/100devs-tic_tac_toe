# 100devs Tic-Tac-Toe Game

This is a simple implementation of the classic Tic-Tac-Toe game using HTML, CSS, and JavaScript. This version can be found in one of the branches of the GitHub repository.

## Program Flow

1. When the DOM content is loaded, the event listener is triggered, and the script starts executing.
2. Query the DOM elements and store them in variables.
3. Initialize variables for the game state.
4. Set up winning conditions in a 2D array.
5. Define functions to handle game logic.
6. Add event listeners to each tile and the reset button.

## Functions

### 1. handleResultValidation()

This function checks if there's a winner or a tie in the game.

1. Iterate through each winning condition.
2. Check if the values in the board array match the winning condition.
3. If a winning condition is met, announce the winner and set isGameActive to false.
4. If there are no empty spaces left and no winner, announce a tie.

### 2. announce(type)

A helper function that displays the game result in the DOM.

- _'type'_: A string representing the game result ("PLAYERX_WON", "PLAYERO_WON", or "TIE").

### 3. isValidAction(tile)

Checks if the selected tile is a valid move.

- _'type'_: The DOM element of the selected tile.

### 4. updateBoard(i)

Updates the board array with the current player's move.

- _'i'_: The index of the selected tile in the board array.

### 5. changePlayer()

Switches the current player between "X" and "O", and updates the player display.

### 6. userAction(tile, i)

Handles user actions on the board.

1. Check if the action is valid and the game is active.
2. Update the selected tile with the current player's symbol.
3. Update the board array.
4. Check for a winner or a tie.
5. Switch the current player.

- _tile_: The DOM element of the selected tile.
- _i_: The index of the selected tile in the board array.

### 7. resetBoard()

Resets the game state, clears the board, and hides the announcer.

1. Reset the board array and isGameActive.
2. Hide the announcer.
3. Reset the current player if needed.
4. Clear the symbols and classes on each tile.

## Event Listeners

5. Add a click event listener to each tile that triggers the userAction() function.
6. Add a click event listener to the reset button that triggers the resetBoard() function.
