# Pacman-Game
Introduction

This project is a Pacman game implemented in C using the SDL (Simple DirectMedia Layer) library. The game follows the classic Pacman mechanics where the player controls Pacman to navigate through a maze, avoid ghosts, and eat pellets.

Features

Graphical Interface using SDL for rendering the game screen.

Character Movement with arrow keys for controlling Pacman.

Sprite Animation for smooth character movements.

Collision Detection for interactions with walls and ghosts.

Game Loop Management to handle events and rendering efficiently.

Custom Map Loading to create different levels.

Requirements

To compile and run the Pacman game, you need:

SDL2 and SDL2_image library installed

C Compiler (GCC recommended)

Windows, Linux, or macOS (with SDL2 support)

Installing SDL2

On Ubuntu/Debian

sudo apt-get install libsdl2-dev libsdl2-image-dev

On macOS (with Homebrew)

brew install sdl2 sdl2_image

On Windows

Download and install SDL2 and SDL2_image from the official SDL website: https://libsdl.org.

Compilation and Execution

Compile the Project

gcc pacman_project.c -o pacman -lSDL -lSDL_image

Run the Game

./pacman

Code Structure

1. Main Game Loop (main())

Initializes SDL.

Loads the game window and assets.

Enters the main event loop for handling player input and updating the game state.

2. load_image() Function

Loads images from the sprites directory and optimizes them for rendering.

3. pacman_sprites() Function

Handles Pacman’s animation and movement.

Uses SDL_BlitSurface() to update Pacman’s sprite based on the direction.

4. gameplay() Function

Runs the game loop.

Calls pacman_sprites() to update Pacman’s position based on key inputs.

Detects quit events to exit the game properly.

5. createmap() Function

Generates the maze layout and obstacles for Pacman.

Controls

Arrow Keys → Move Pacman in respective directions.

Esc → Exit the game.

Possible Enhancements

Implement Ghost AI for challenging gameplay.

Add Power Pellets to allow Pacman to defeat ghosts.

Improve collision detection with walls.

Introduce multiple levels with increasing difficulty.

Implement high score tracking.
