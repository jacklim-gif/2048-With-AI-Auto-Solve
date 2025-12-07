⚡ 2048 AI Auto-Solver 🤖🧩

A smart, beautiful, and fully automated 2048 experience powered by Expectimax AI.

A modern re-creation of the classic 2048 game — but upgraded with an intelligent Auto-Solver, smooth neon UI, animations, and smart search heuristics that reach 2048/4096 with ease.

This project is fully open-source and built with pure HTML + CSS + JavaScript, no frameworks needed.

👥 Contributors

Jack – Full AI Logic, Game Engine, UI/UX

(Optional) Add more contributors if needed

✨ Features

Expectimax AI Engine
The bot calculates the best move using probability-weighted outcomes (90% tile = 2, 10% tile = 4).

Smart “Snake Pattern” Heuristics
✔ Monotonicity
✔ Smoothness
✔ Empty cell weighting
Makes the AI survive longer and reach bigger tiles.

Dynamic Survival Mode
Normal state → depth 4
Critical state (≤4 empty tiles) → depth 6

Auto-Solver Mode
Watch the AI instantly take over and clear the board.

Glassmorphism UI + Neon Effects
Smooth tile animations, blur effects, glowing highlights.

Fast-Win Demo Mode
Spawns larger tiles for quick testing or recording videos.

Fully Responsive
Works on desktop + mobile with smooth scaling.

No Backend Needed
100% front-end, open and portable.

🧠 How the AI Works
1. Expectimax Search

Because 2048 has randomness, it uses chance-based decision trees:

Max Layer (AI turn): Chooses the best move (Up/Down/Left/Right)

Chance Layer (Game): Simulates random tile drops

This allows deeper, more accurate predictions than Minimax.

2. Heuristic Evaluation

Every board is scored using:

Monotonicity:
Encourages snake pattern so large tiles stay aligned.

Smoothness:
Penalties for huge jumps between adjacent tiles.

Empty Tiles:
More space = fewer deadlocks.

3. Survival Mode

When the board is nearly full, the AI automatically switches to a deeper search to avoid losing.

🕹️ Live Demo

(Optional: Replace this with GitHub Pages link)
👉 Play the Game Here

⚙️ Configuration

You can fine-tune AI behavior in one file:

const CONFIG = {
    size: 4,
    aiDelay: 150,
    aiDepth: 4,
    survivalDepth: 6
};

🛠️ Tech Stack

Pure JavaScript (Vanilla) — no dependencies

HTML5 Canvas + CSS Animations

Neon/Glassmorphism UI

Local rendering engine

🚀 Run Locally
# 1. Clone the repo
git clone https://github.com/jacklim-gif/2048-With-AI-Auto-Solve.git
cd 2048-With-AI-Auto-Solve

# 2. Open the game
# Just double-click the file:
game.html


No build. No install. No dependencies.
Just open and play.

🤝 Contributing
Fork → Create Branch → Commit → Push → Pull Request

📜 License

MIT License — free for personal + commercial use.

<div align="center">
💙 Built with focus, fun, and code by Jack Lim

Want me to help you add:
✔ A banner image
✔ A gameplay GIF
✔ Shields.io badges
✔ Icon sections
✔ Dark neon theme enhancements

Just tell me — I can style it exactly the way you want.

</div>
