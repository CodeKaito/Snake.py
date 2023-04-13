# Snake Game

This is a simple implementation of the classic Snake game using the Pygame library. The game initializes with a window size of 1380 x 960 and a square size of 30. The snake starts at position [120,60] moving in the "RIGHT" direction.

The game includes the following elements:
- Snake body: The body is drawn as a green rectangle whose coordinates change according to the head movement.
- Food: The food is drawn as a red rectangle that is randomly placed within the game window. Whenever the snake's head reaches the food, its length increases by one, and a new food is spawned.
- Score: The score is displayed at the top left corner of the game window and increases by one for each food that is consumed.
- Speed: The speed of the snake also increases every 5 scores (speed = 15 + 2*number of times score is a multiple of 5), but it will not drop below 15.


The game is run in an infinite `while` loop, with the game window being updated after every move. The snake moves in the direction indicated by the `direction` variable, which is updated according to keyboard inputs.

If the snake collides with the game window's border or with its body, the game restarts, and the score is set back to zero.

Overall, the code implements a basic version of the classic Snake game using the Pygame library. Here is a breakdown of the different components:

Import statements: The code imports the Pygame, sys, time, and random libraries.

Global variables: The code defines global variables for the speed of the game and the size of the game window.

Initialization: The code initializes the Pygame library and checks for any errors. It also sets the title of the game window and creates the game window.

Helper functions: The code defines two helper functions for displaying the score and speed of the game. These functions take arguments for the color, font, and size of the text.

Game setup: The code initializes variables for the position of the snake's head, the snake's body, the position of the food, whether the food has been spawned, the score, and the direction of the snake.

Game loop: The code enters an infinite loop that handles user input, updates the position of the snake, checks for collisions with the food and the body of the snake, and updates the score and speed of the game. The loop also displays the graphics for the game, including the snake, the food, the score, and the speed.

Game over: If the head of the snake collides with the body, the game resets and the loop starts again.
