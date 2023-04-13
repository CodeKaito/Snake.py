# Snake Game

This is a simple implementation of the classic Snake game using the Pygame library. The game initializes with a window size of 1380 x 960 and a square size of 30. The snake starts at position [120,60] moving in the "RIGHT" direction.

The game includes the following elements:
- Snake body: The body is drawn as a green rectangle whose coordinates change according to the head movement.
- Food: The food is drawn as a red rectangle that is randomly placed within the game window. Whenever the snake's head reaches the food, its length increases by one, and a new food is spawned.
- Score: The score is displayed at the top left corner of the game window and increases by one for each food that is consumed.
- Speed: The speed of the snake also increases every 5 scores (speed = 15 + 2*number of times score is a multiple of 5), but it will not drop below 15.


The game is run in an infinite `while` loop, with the game window being updated after every move. The snake moves in the direction indicated by the `direction` variable, which is updated according to keyboard inputs.

If the snake collides with the game window's border or with its body, the game restarts, and the score is set back to zero.

Overall, this code provides a good implementation of the classic snake game using Pygame library.
