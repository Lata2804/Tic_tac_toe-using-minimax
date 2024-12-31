# Tic_tac_toe-using-minimax

This is a Python-based implementation of the classic Tic-Tac-Toe game, enhanced with an AI opponent using the Minimax algorithm. The game supports a human player versus the AI.

---

## Features

- **Interactive gameplay**: Players can choose their moves by entering numbers corresponding to board positions. Here's a visual representation of the board layout:

```
 1 | 2 | 3
---|---|---
 4 | 5 | 6
---|---|---
 7 | 8 | 9
```

- **AI opponent**: The AI utilizes the Minimax algorithm for optimal decision-making.
- **Customizable symbols**: Players can choose between `X` or `O` as their symbol.
- **Replay option**: Play multiple rounds in a single session. The board resets automatically after each round, and players can choose whether to continue or exit.
- **Winning detection**: The game automatically detects win, loss, or draw scenarios.

---

## How to Play
1. **Choose your symbol**: The game starts by asking you to choose your symbol (`X` or `O`). `X` always goes first.
2. **Make your move**: Enter the number corresponding to the position on the board where you'd like to place your symbol. The positions are numbered as follows:

```
 1 | 2 | 3
---|---|---
 4 | 5 | 6
---|---|---
 7 | 8 | 9
```

   - If you input an invalid number (e.g., a number outside the range 1–9 or a position that is already occupied), the game will prompt you to enter a valid number until a correct input is provided.

3. **AI Move**: The AI will make its move based on the Minimax algorithm.
4. **Game outcome**: The game ends when there is a winner or the board is full. You can then choose to play again or exit.

---

## Code Structure

- **`disp` Class**: Handles the display of the Tic-Tac-Toe board.
- **`pos` Class**: Contains helper functions for checking win conditions, open spots, and closed spots on the board.
- **`minimax` Class**: Implements the Minimax algorithm for the AI. The Minimax algorithm works by simulating all possible moves and counter-moves to determine the optimal strategy for the AI. It assigns scores to game states, aiming to maximize the AI's chances of winning while minimizing the opponent's chances.
- **Main Game Loop**: Handles player input, AI moves, and game progression.

---

## Getting Started

### Prerequisites

- Python 3.x installed on your system.

### Running the Game

1. Clone this repository:
   ```bash
   git clone https://github.com/Lata2804/Tic_tac_toe-using-minimax.git
   ```
2. Navigate to the project directory:
   ```bash
   cd Tic_tac_toe-using-minimax
   ```
3. Run the script:
   ```bash
   python minimaxai.py
   ```

---

## Example Gameplay

```
X or O? (X goes first)
>>> X

 1 | 2 | 3
---|---|---
 4 | 5 | 6
---|---|---
 7 | 8 | 9

Input number of square you'd like to move to:
>>> 5

AI chooses square 1

 O | 2 | 3
---|---|---
 4 | X | 6
---|---|---
 7 | 8 | 9

Input number of square you'd like to move to:
>>> 3

AI chooses square 7

 O | 2 | X
---|---|---
 4 | X | 6
---|---|---
 O | 8 | 9

Input number of square you'd like to move to:
>>> 2

AI chooses square 4

 O | X | X
---|---|---
 O | X | 6
---|---|---
 O | 8 | 9

AI win!

Play again? Yes/No:
>>> no
```

You win!

Play again? Yes/No:
>>> no
```

---


## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## Contributing

Contributions are welcome! Feel free to fork the repository and submit a pull request with your improvements.
