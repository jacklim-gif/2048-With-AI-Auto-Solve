2048 AI Auto-Solver 🤖🧩

A high-performance implementation of the classic 2048 game featuring an intelligent Auto-Solve AI.
The AI uses the Expectimax Algorithm with heuristic optimizations to consistently reach 2048 and beyond.

🎮 Live Demo

(Optional: Replace with your GitHub Pages link)
👉 Play the Game

🧠 How the AI Works

This AI strategically analyzes future moves instead of picking random directions.

1. Expectimax Algorithm

2048 has randomness (new tiles spawn unpredictably), so the AI uses Expectimax, not Minimax.

Max Nodes (Player): Chooses the best move.
Chance Nodes (Environment): Calculates random tile spawns:

90% → 2

10% → 4

2. Heuristic Evaluation ("Snake Strategy")

The AI scores the board using:

Monotonicity — Encourages a snake-like pattern with the largest tile in a corner

Smoothness — Penalizes large jumps between adjacent tiles

Empty Cells — Rewards having space to survive longer

3. Dynamic Survival Mode
Game State	AI Depth
Normal board	4 moves deep
Critical state (less than 4 empty tiles)	6 moves deep

This helps the AI escape near-loss situations.

✨ Features

⚡ Auto-Solver (plays for you)

🎨 Polished UI with animations

⏩ Fast-Win Mode

🧠 Reaches 2048 / 4096 commonly

📱 Responsive for mobile

🛠️ No frameworks — pure HTML/CSS/JS

🚀 Getting Started
1. Clone the Repository
git clone https://github.com/jacklim-gif/2048-With-AI-Auto-Solve.git

2. Run the Game

Just open game.html in any browser.

No installation needed.

🛠️ Configuration

You can tweak the AI in the CONFIG object:

const CONFIG = {
    size: 4,
    aiDelay: 150,
    aiDepth: 4,
    survivalDepth: 6
};

🤝 Contributing

Fork the repo

Create a branch

git checkout -b feature/MyFeature


Commit changes

git commit -m "Add feature"


Push the branch

git push origin feature/MyFeature


Open a Pull Request

📝 License

Distributed under the MIT License.
See the LICENSE file for details.

Built with ❤️ by Jack Lim
