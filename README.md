# Simon Says Game: A Raspberry Pi and LED Project

This project replicates the classic **Simon Says** memory game using a Raspberry Pi, LEDs, and buttons. The game challenges players to memorize and replicate an increasing sequence of colors, testing their memory and speed.

## Project Overview

In this project:
- **LEDs** represent the colors in the Simon Says game.
- **Buttons** allow players to input their responses.
- A **Raspberry Pi** handles the game logic, including generating random sequences, verifying user input, and managing the game's progression.
- The game is coded in Python and uses the RPi.GPIO library for GPIO pin control.

## Features

- **Interactive Gameplay**: LEDs light up in a specific sequence, which players must replicate using buttons.
- **Random Patterns**: The sequence increases in length and complexity with each level.
- **Speed Variation**: Adjustable game speed to increase difficulty.
- **Real-Time Feedback**: Immediate response to user input with visual (LED flashes) and optional audio feedback.
- **Game Over and Restart**: Tracks the highest score and allows players to restart after a game over.

## How It Works

1. **Game Start**:
   - The game initializes the GPIO pins for LEDs and buttons.
   - A random sequence of colors is generated.

2. **Pattern Display**:
   - LEDs flash in the pattern that the player must memorize.

3. **Player Input**:
   - Players press buttons corresponding to the LEDs' pattern.
   - The program verifies each input in real-time.

4. **Progression**:
   - If the player completes the sequence, the pattern grows longer, and the game continues.
   - If the player inputs incorrectly, the game ends, displaying the score.

## Hardware Requirements

- **Raspberry Pi** (any model with GPIO pins)
- **4 LEDs** (different colors: green, red, blue, yellow)
- **4 Push Buttons**
- **Resistors** for LEDs and buttons
- Breadboard and jumper wires
- Power supply for the Raspberry Pi

### GPIO Pin Mapping

| Component   | GPIO Pin  | Color       |
|-------------|-----------|-------------|
| Green LED   | 33        | Green       |
| Red LED     | 37        | Red         |
| Blue LED    | 35        | Blue        |
| Yellow LED  | 31        | Yellow      |
| Green Button| 11        | Green       |
| Red Button  | 15        | Red         |
| Blue Button | 13        | Blue        |
| Yellow Button| 7        | Yellow      |

