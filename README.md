# Chess Enigma

Chess Enigma is a Python-based chess game that combines an interactive graphical interface with a simple AI opponent. The AI leverages the minimax algorithm with alpha-beta pruning and evaluates moves using both material balance and piece-square tables to determine optimal strategies.

## Project Structure

- **Main.py**  
  The entry point of the game. It initializes the chess board, handles user input, and manages the game loop. Depending on the player's chosen color, it invokes the AI (via the minimax algorithm) to make moves.

- **Board.py**  
  Contains the `DisplayBoard` class responsible for rendering the chessboard using Pygame. This file also includes the `Piece` class to load and display chess pieces.

- **Evaluation.py**  
  Implements the `Evalualtion` class, which evaluates board positions based on material, piece development, and game stage (early or late game).

- **MiniMax.py**  
  Implements the minimax algorithm with alpha-beta pruning. This file recursively explores potential moves using the evaluation function from `Evaluation.py` to determine the best move for the AI.

- **Piece_Devolopment_values.py**  
  Defines the `BoardValues` class, which contains piece-square tables that assign positional scores to pieces. These values guide the AI's decision-making process.

## Requirements

- **Python 3.x**
- **pygame** – for graphical interface and event handling
- **python-chess** – for board representation and move generation

## Setup and Installation

1. **Clone the repository or download the source files.**

2. **Install the required packages using pip:**

   ```bash
   pip install -r requirements.txt
   

## Running the Game

To start the game, simply run:

```bash
python Main.py
```

A game window will open displaying the chessboard. Use the left mouse button to select and move pieces, and the right mouse button to deselect a chosen piece.

Enjoy playing Chess Enigma!
```
