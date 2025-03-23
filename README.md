Rusty Ping Pong Game
==============

Overview
--------

This project is a simple Ping Pong game built using the **Bevy** game engine in Rust. It features AI-controlled paddles, collision detection, scoring, and a moving ball.

Features
--------

*   **Player and AI-controlled paddles**
    
*   **Ball movement with physics-based collision detection**
    
*   **Score tracking and display**
    
*   **Automatic ball reset after scoring**
    
*   **Simple AI opponent**
    
*   **Rendered using Bevy's 2D engine**
    

Installation
------------

### Prerequisites

Ensure you have **Rust** and **Cargo** installed. You can install Rust using [rustup](https://rustup.rs/):

`   curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh   `

### Clone the Repository

`   git clone   cd rusty-ping-pong   `

### Run the Game

`   cargo run   `

### Controls

- **Arrow Up (↑)**: Move paddle up.
- **Arrow Down (↓)**: Move paddle down.

Code Structure
--------------

### Components

- **Ball**: Represents the game ball.
- **Paddle**: Represents paddles (Player and AI).
- **Player**: Represents the player's paddle.
- **Ai**: Represents the AI paddle.
- **Score**: Tracks the player's and AI's scores.
- **Velocity**: Controls movement of the ball and paddles.
- **Position**: Stores entity positions.
- **Shape**: Defines object shapes.

### Systems

- **move_ball**: Updates ball movement.
- **move_ai**: Moves AI paddle.
- **handle_player_input**: Controls player movement.
- **detect_scoring**: Detects when a goal is scored.
- **update_score**: Updates score values.
- **update_scoreboard**: Updates the on-screen scoreboard.
- **handle_collisions**: Handles ball collisions with paddles and walls.
- **reset_ball**: Resets the ball after scoring.
- **spawn_ball, spawn_paddles, spawn_gutters, spawn_scoreboard, spawn_camera**: Initialize game objects.

Dependencies
------------

*   [Bevy](https://bevyengine.org/) - A fast, modern Rust game engine
    

Contributing
------------

Pull requests are welcome! For major changes, please open an issue first to discuss.

License
-------

This project is licensed under the MIT License. See LICENSE for details.
