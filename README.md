# Snake-game
# Snake Game in Java

This project is a classic Snake game implemented in Java. The game features a snake that moves around a grid, eating fruit to grow longer, and the player controls the snake using the keyboard. The game ends if the snake collides with the walls or itself.

## Features

* **Classic Snake Gameplay:** Control the snake to eat fruit and avoid collisions.
* **Score Tracking:** Keeps track of the player's score and the number of fruits eaten.
* **Game States:** Supports different game states like new game, game over, and pause.
* **Keyboard Controls:** Players use the W/A/S/D or arrow keys to control the snake's direction.
* **Game Speed Control:** The game's speed is managed using a `Clock` class.
* **GUI Implementation:** The game uses Swing for the graphical user interface.

## How to Run

1.  **Prerequisites:**
    * Java Development Kit (JDK) installed.

2.  **Compilation:**
    * Compile the Java files. You can do this from the command line using `javac \*.java` or use an IDE like IntelliJ IDEA or Eclipse.

3.  **Execution:**
    * Run the `SnakeGame.java` file to start the game.  From the command line, this is typically done using `java SnakeGame`.

## Game Controls

* **Move Up:** W or Up Arrow key
* **Move Down:** S or Down Arrow key
* **Move Left:** A or Left Arrow key
* **Move Right:** D or Right Arrow key
* **Pause Game:** P
* **Start New Game/Restart:** Enter

## Code Structure

The project is structured into several Java classes:

* `SnakeGame.java`: This is the main class that initializes and runs the game. It handles the game loop, user input, and game logic. [cite: 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 53, 54, 55, 56, 57, 58, 59, 60, 61, 62]
* `BoardPanel.java`: This class is responsible for drawing the game board, including the snake, fruit, and background.
* `SidePanel.java`: This class displays the game's statistics (score, fruits eaten, etc.) and controls. [cite: 102, 103, 104, 105, 106]
* `Direction.java`: An enum defining the possible directions the snake can move (North, East, South, West). [cite: 116]
* `TileType.java`: An enum representing the different types of tiles on the game board (Fruit, SnakeHead, SnakeBody). [cite: 117]
* `Clock.java`:  This class manages the game's timing and update cycles. [cite: 118, 119, 120, 121, 122]

## Game Logic

The game logic is primarily handled in the `SnakeGame.java` and `Clock.java` files.

* **Game Loop:** The `startGame()` method in `SnakeGame.java` contains the main game loop, which updates the game state and renders the game at a fixed frame rate. [cite: 21, 22, 23, 24, 25, 26, 27, 28, 29, 70, 71, 72, 73, 74, 75]
* **Snake Movement:** The `updateSnake()` method in `SnakeGame.java` updates the snake's position based on the current direction. It also handles collision detection (with walls and itself). [cite: 33, 34, 35, 36, 37, 38, 78, 79, 80, 81, 82]
* **Fruit Spawning:** The `spawnFruit()` method in `SnakeGame.java` generates new fruit at random locations on the board. [cite: 45, 46, 47, 92, 93, 94, 95, 96, 97]
* **Collision Detection:** The `updateSnake()` method checks for collisions between the snake and the walls or itself. If a collision occurs, the game is over. [cite: 30, 31, 32]
* **Scoring:** The player's score increases when the snake eats fruit. The `score` and `fruitsEaten` variables in `SnakeGame.java` track the player's progress. [cite: 32, 76, 77]
* **Pausing:** The game can be paused and resumed using the 'P' key. The `isPaused` flag in `SnakeGame.java` and the `Clock.java` are used to manage the pause state. [cite: 19, 43, 44, 68, 122, 123, 124, 125, 126, 127, 128, 129, 130, 131, 132, 133, 134, 135, 136, 137]
* **Game Reset:** The `resetGame()` method in `SnakeGame.java` resets the game to its initial state. [cite: 39, 40, 41, 83, 84, 85, 86, 87]
