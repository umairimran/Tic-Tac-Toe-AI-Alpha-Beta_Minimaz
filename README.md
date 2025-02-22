# 🧩 **Tic-Tac-Toe AI with Alpha-Beta Pruning** 🤖

## 🎮 **Overview**
Welcome to the **Tic-Tac-Toe AI** project! This Python-based implementation allows you to play a classic game of Tic-Tac-Toe against a highly intelligent AI. The AI is powered by the **Minimax Algorithm** combined with **Alpha-Beta Pruning**, making it a formidable opponent that can think several moves ahead.

Whether you're a beginner or an experienced player, this game will offer a challenging and fun experience. 🏆

---

## 🚀 **Key Features**
- **AI vs Human Mode**: Compete against a smart AI (X) or play as a human (O).
- **Optimized AI with Alpha-Beta Pruning**: The AI uses Alpha-Beta Pruning to minimize unnecessary computations, speeding up decision-making and ensuring optimal moves.
- **Interactive Console Interface**: Play via a simple and user-friendly console interface.
- **Game State Detection**: Automatically detects whether the game has ended in a win, loss, or draw.

---

## 🕹️ **Game Flow**
1. **Game Initialization**: The board is initialized with all spaces empty.
2. **Alternating Turns**: The game alternates turns between the human player and the AI.
3. **AI Turn**: The AI calculates the optimal move using **Minimax with Alpha-Beta Pruning** and places its move on the board.
4. **Human Turn**: The human player selects an empty cell by entering the row and column.
5. **Game End**: The game continues until either player wins or the game ends in a draw.

---

## 🏁 **Player Modes**
- **Human Player (O)**: You, the human player, will input your move by specifying the row and column numbers (e.g., `0 2` for the top-right corner).
- **AI Player (X)**: The AI (represented by `X`) makes optimal decisions using the **Minimax Algorithm** enhanced with **Alpha-Beta Pruning**.

---

## 🧠 **Tech Stack**
- **Python 3**: The primary programming language for this project.
- **Minimax Algorithm**: An algorithm used to evaluate and select the best move.
- **Alpha-Beta Pruning**: An optimization technique used in conjunction with Minimax to cut down on unnecessary branches, speeding up the AI's decision-making process.

---

## 📜 **Code Breakdown**

### Key Functions:
- **`initial_state()`**: Initializes the empty game board (3x3 grid).
- **`player(board)`**: Determines which player’s turn it is based on the board’s current state.
- **`actions(board)`**: Returns all possible legal moves based on the current game board.
- **`terminal(board)`**: Checks whether the game has reached a terminal state (win or draw).
- **`utility(board)`**: Returns the utility of the current board:
    - `1` if AI wins.
    - `-1` if Human wins.
    - `0` for a draw.
- **`minmax(board, symbol)`**: Implements the **Minimax Algorithm** to compute the optimal move.
- **`alpha_beta_pruning(board)`**: A placeholder for the alpha-beta pruning logic (implemented inside `minmax` and `get_maxmin_score`).

### **Minimax with Alpha-Beta Pruning**:
The AI evaluates all potential moves and uses **alpha-beta pruning** to eliminate branches of the game tree that don't need to be explored, ensuring a faster decision-making process. This results in the AI making its decisions in a fraction of the time, even on complex boards.

---

## 🎮 **Sample Output**

```plaintext
Player O (Human) has these options to choose:
{(0, 1), (1, 1), (2, 1), (1, 0), (0, 2), (1, 2), (2, 0)}
You have these options to choose:
Enter row and column (0-2) separated by space: 0 0
