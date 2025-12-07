<div align="center">

2048 AI Auto-Solver 🤖🧩

A high-performance, autonomous 2048 bot powered by the Expectimax Algorithm.





Watch the AI predict, strategize, and win.

🎮 Play the Live Demo





(Click above to play instantly in your browser)

</div>

🧠 How the AI Works

This isn't just a random move generator. The AI "thinks" about future board states using advanced game theory concepts derived from chess engines.

1. Expectimax Algorithm

Unlike Chess (which uses Minimax), 2048 is a game of chance because new tiles spawn randomly. I implemented Expectimax to handle this stochastic nature:

Max Nodes (Player): The AI evaluates the best move (Up, Down, Left, Right).

Chance Nodes (Environment): The AI calculates the average outcome of all possible random tile spawns (90% chance of '2', 10% chance of '4').

2. Heuristic Evaluation (The "Snake" Strategy)

The AI evaluates board states based on specific criteria to keep the grid organized:

🐍 Monotonicity: Forces the values to increase in a snake-like pattern (e.g., largest tile in the bottom-right corner).

🌊 Smoothness: Penalizes adjacent tiles that have drastically different values to ensure they can merge easily.

🔲 Empty Cells: Rewards keeping the board open to prevent "Game Over" scenarios.

3. Dynamic "Survival Mode"

To balance performance and intelligence:

Standard Play: The AI searches 4 moves deep.

Survival Mode: If the board becomes critical (less than 4 empty cells), the AI automatically deepens its search to 6 moves to find a precise escape route.

✨ Features

Feature

Description

⚡ Auto-Solve

Watch the AI play in real-time with superhuman efficiency.

🎨 Smooth UI

Glassmorphism design with silky CSS animations for sliding and merging.

⏩ Demo Mode

Optional "Fast Win" mode that spawns larger numbers (great for recording).

🏆 Intelligent

Capable of reaching the 2048 tile (and often 4096) autonomously.

📱 Responsive

Fully optimized for Desktop and Mobile touchscreens.

🚀 Getting Started

No installation, build steps, or backend required. This project is built with pure vanilla web technologies.

1. Clone the repository

Open your terminal and run:

git clone [https://github.com/jacklim-gif/2048-With-AI-Auto-Solve.git](https://github.com/jacklim-gif/2048-With-AI-Auto-Solve.git)


2. Open the Game

Simply locate the folder and double-click game.html to open it in your browser (Chrome, Edge, Firefox, etc.).

🛠️ Configuration

You can tweak the AI's behavior by modifying the CONFIG object inside the game.html source code:

const CONFIG = {
    size: 4,           // Grid size (4x4)
    aiDelay: 150,      // Speed of AI moves in milliseconds
    aiDepth: 4,        // Standard lookahead depth (Intelligence)
    survivalDepth: 6   // Lookahead depth when in danger (Panic Mode)
};


🤝 Contributing

Contributions are welcome! If you have ideas for better heuristics or optimization:

Fork the Project

Create your Feature Branch (git checkout -b feature/AmazingFeature)

Commit your Changes (git commit -m 'Add some AmazingFeature')

Push to the Branch (git push origin feature/AmazingFeature)

Open a Pull Request

📝 License

Distributed under the MIT License. See LICENSE for more information.

<div align="center">





Built with ❤️ by <a href="https://www.google.com/search?q=https://github.com/jacklim-gif">Jack Lim</a>
</div>
