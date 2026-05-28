# ✂️ Rock Paper Scissors Game

A console-based C++ Rock Paper Scissors game where you play against the computer across multiple rounds.

---

## 📖 Overview

Rock Paper Scissors is an interactive command-line application where the player competes against a computer opponent over 3 rounds per game. The computer makes random choices each round, and the overall game winner is determined by the most round wins.

---

## ✨ Features

- **Player vs Computer**: Computer picks randomly each round
- **3 Rounds Per Game**: Best of 3 determines the game winner
- **Round-by-Round Results**: Detailed breakdown after each round
- **Draw Detection**: Handles ties at both round and game level
- **Replay Option**: Play as many games as you want without restarting the program

---

## 🎮 How to Play

1. Run the program.
2. Each round, choose your move:
   - `1` Stone
   - `2` Paper
   - `3` Scissors
3. The computer makes its move randomly.
4. See the result of each round instantly.
5. After 3 rounds, the overall game winner is announced.
6. Choose whether to play again.

---

## 📊 Winning Rules

| Player Choice | Computer Choice | Winner |
|---|---|---|
| Stone | Scissors | Player 1 |
| Paper | Stone | Player 1 |
| Scissors | Paper | Player 1 |
| Same | Same | Draw |

The player with the most round wins takes the game. If equal, it's a Draw.

---

## 🏗️ Project Structure

```
RockPaperScissors/
│
├── main.cpp          # Full source code
└── README.md         # Project documentation
```

### Key Components

| Component | Description |
|---|---|
| `enGameChoice` | Enum for player choices (Stone, Paper, Scissors) |
| `enWinner` | Enum for round/game outcome (Player1, Computer, Draw) |
| `stRoundInfo` | Struct holding individual round data |
| `stGameResults` | Struct holding the full game session results |
| `GetComputerChoice()` | Generates a random move for the computer |
| `WhoWonTheRound()` | Evaluates the winner of a single round |
| `WhoWonTheGame()` | Determines the overall game winner |
| `PlayGame()` | Runs the full game loop across all rounds |
| `StartGame()` | Entry point with replay support |

---

## ⚙️ Requirements

- **Compiler**: Any C++11-compatible compiler (e.g., GCC, MSVC, Clang)
- **OS**: Windows (uses `system("cls")` for screen clearing)

---

## 🚀 Getting Started

### Compile

```bash
g++ main.cpp -o RockPaperScissors
```

### Run

```bash
./RockPaperScissors
```

> ⚠️ **Note**: The screen-clearing feature relies on the Windows console command (`cls`). On Linux/macOS, this call will have no effect but the game will still run correctly.

---

## 🔮 Possible Improvements

- Allow the player to choose the number of rounds
- Add a score history across multiple games
- Replace `system()` calls with cross-platform alternatives
- Add a best-of-N mode

---

## 📄 License

This project is open source and free to use for educational purposes.

---

## 👤 Author

👤 **Ahmed Mohamed**  
📧 ahmed.mohamed@example.com  
💼 [linkedin.com/in/ahmed-mohamed](https://linkedin.com/in/ahmed-mohamed)
