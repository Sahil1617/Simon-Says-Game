#Color Sequence Memory Game

Overview:
This project is a color sequence memory game inspired by Simon Says. Players must memorize and reproduce an increasingly complex sequence of colors. As the game progresses, the level increases, challenging the user's memory and attention.


Features:
1. Game Flow
Starts with a random color in the sequence.
On each level, a new random color is added to the sequence.
The user must click the colors in the correct order to proceed.
2. Interactive Buttons
Four buttons (yellow, red, green, purple) serve as the game inputs.
Visual effects for both system-generated and user-generated flashes make gameplay dynamic.
3. Score Display
Displays the current level during the game.
Shows the final score after a game-over event.
4. Reset Mechanism
The game resets automatically after a wrong sequence and displays an option to restart.


How to Play:
Start the Game:
Press any key to begin the game.
A random color sequence will flash.

Repeat the Sequence:
Click the buttons in the correct order as shown by the sequence.

Advance to the Next Level:
If the sequence is correct, the game will add another color to the sequence, increasing the level.

Game Over:
If a mistake is made, the game ends, and the score (level reached) is displayed.
Press any key to restart.


Code Highlights:
Game Logic:
gameSeq holds the generated sequence for each level.
userSeq tracks the user's input.

Flashing Effects:
gameFlash(btn) visually highlights the game's generated button sequence.
userFlash(btn) provides feedback for user clicks.

Level Progression:
levelUp() adds a new random color to the sequence and updates the display.

Answer Validation:
checkAns(idx) checks the user's input against the game's sequence. If correct, the game proceeds; otherwise, it resets.

Reset Mechanism:
The reset() function resets all variables to their initial state.