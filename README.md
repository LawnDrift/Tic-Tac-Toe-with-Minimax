# Tic Tac Toe with Minimax

This project is a web-based version of the famous game Tic Tac Toe, built with **CSS, HTML, and Javascript**.
The AI opponent was made using the **Minimax algorithm**, which is a decision-making algorithm used in two-player turn-based games. 

It works by simulating all possible moves and their outcomes, 
assuming both players play optimally. The AI chooses the move that maximizes its own chance of winning while minimizing the opponent’s — hence the name "Minimax."
This makes the AI very challenging to beat. The best a human player can achieve against this AI is a tie.

[👉Play it here](https://lawndrift.github.io/Tic-Tac-Toe-with-Minimax/minimax-tic-tac-toe/tic_tac_toe.html)

## Screenshot
<img src="minimax-tic-tac-toe/tic tac toe screenshot.png" height="500px">

## 🧠 How It Works

The AI uses the **Minimax algorithm** to evaluate the best possible move at each turn. Difficulty levels are implemented by limiting the depth of the Minimax search:

- **Easy** – random moves
- **Medium** – Minimax with limited depth (e.g., 1).
- **Impossible** – full-depth Minimax (perfect play)

The game saves your selected symbol (X or O) and difficulty using `localStorage`, so it remembers your preferences across sessions.

Some extra features to this game include:
- **Hover Effect** - Whenever you hover a cell from the board, you get a preview of your selected symbol (X or O).
- **Scores** - There were added computer, draw, and player scores for whenever the game ends with either the player or computer winning, or ending in a tie.
- **Simple UI** - Intuitive User Interface.

## 🕹️ How to Play

Choose your symbol — X or O — by clicking one of the buttons at the top.

1. Select the difficulty — Easy, Medium, or Impossible.

2. Play your turn by clicking on an empty cell in the 3×3 grid.

3. The AI will respond after a short "thinking" delay.

4. The game ends when either player gets three in a row, column, diagonal, or the board is full (a draw).

5. Click Play Again to restart the round and keep score, or change settings to start fresh.

## 🛠️ Customization & Tweaks

If you want to modify or build on top of this game, here are some ideas:

- 💡 Change the board size (currently 3x3)
- 🎨 Customize the UI theme or animations, you can also canvas graphics or webGl to customize.
- 🧪 Improve the AI: Add alpha-beta pruning to save time when it comes to looking every possible move.
- 🎮 Add a 2-player mode

All the core game logic is in `tic_tac_toe.js`. The AI logic is inside the `bestMove()` and `minimax()` functions.

## Contributing

Feel free to fork this repo and experiment! Pull requests and suggestions are welcome.

## 📄 License

MIT – do whatever you want with it, just give credit if you share something awesome.
