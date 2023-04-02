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

### handleResultValidation()

This function checks if there's a winner or a tie in the game.

    Iterate through each winning condition.
    Check if the values in the board array match the winning condition.
    If a winning condition is met, announce the winner and set isGameActive to false.
    If there are no empty spaces left and no winner, announce a tie.

### announce(type)

A helper function that displays the game result in the DOM.

    type: A string representing the game result ("PLAYERX_WON", "PLAYERO_WON", or "TIE").

### isValidAction(tile)

Checks if the selected tile is a valid move.

    tile: The DOM element of the selected tile.

### updateBoard(i)

Updates the board array with the current player's move.

    i: The index of the selected tile in the board array.

### changePlayer()

Switches the current player between "X" and "O", and updates the player display.
userAction(tile, i)

Handles user actions on the board.

    Check if the action is valid and the game is active.
    Update the selected tile with the current player's symbol.
    Update the board array.
    Check for a winner or a tie.
    Switch the current player.

    tile: The DOM element of the selected tile.
    i: The index of the selected tile in the board array.

### resetBoard()

Resets the game state, clears the board, and hides the announcer.

    Reset the board array and isGameActive.
    Hide the announcer.
    Reset the current player if needed.
    Clear the symbols and classes on each tile.

## Event Listeners

    Add a click event listener to each tile that triggers the userAction() function.
    Add a click event listener to the reset button that triggers the resetBoard() function.
