# simon-game
Simon Game Using JQuery
This code implements a simplified version of the Simon game:

- **Game Setup:**
  - Four button colors are defined: red, blue, green, and yellow.
  - Arrays `gamePattern` and `userClickedPattern` store the generated and user-input color sequences.
  - Variables `started` and `level` track the game state and current level.

- **Game Initialization:**
  - The game starts when a key is pressed (`$(document).keypress`).
  - The `nextSequence` function initiates the first level, showing a random color and playing a sound.

- **User Interaction:**
  - When a colored button is clicked (`$(".btn").click`), the user's chosen color is recorded.
  - The `checkAnswer` function compares the user's input to the generated sequence, progressing to the next level if correct.

- **Feedback and Animation:**
  - Animation functions (`animatePress` and `nextSequence`) provide visual feedback by highlighting and briefly fading the colored buttons.
  - The `playSound` function plays corresponding audio files for each color.

- **Game Over Handling:**
  - If the user makes a mistake, a "Game Over" message is displayed, and the game resets after a brief delay.

- **Game Restart:**
  - The `startOver` function resets the game variables, allowing the user to restart by pressing any key after a game over.

This code uses jQuery for DOM manipulation and provides a basic interactive Simon game experience.
