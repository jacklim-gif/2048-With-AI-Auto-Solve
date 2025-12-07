🎮 2048 AI Auto-Solver 🤖🧩

A smart 2048 game clone powered by an intelligent Auto-Solve bot.

<div align="center">
🚀 Built with Vanilla JavaScript • 🧠 Expectimax AI • 🎨 Smooth UI
<br>


(You can replace this banner with your own image)

</div>
⭐ Features

⚡ Auto-Solver — Watch the AI complete the game for you

🧠 Expectimax Algorithm — Not random, but real decision-making

🐍 Snake-Pattern Heuristic for smarter tile organization

🎨 Glass UI + Clean Animations

⏩ Fast-Win Demo Mode

📱 Responsive Design

🛠️ Pure HTML + CSS + JS (no frameworks)

🧠 How the AI Thinks
🔹 1. Expectimax Algorithm

Because new tiles spawn randomly, the AI evaluates:

Max Nodes → Best move the player can make

Chance Nodes → Random spawn:

90% = 2

10% = 4

This gives the AI the ability to “see the future” more accurately.

🔹 2. Heuristic Scoring

The AI grades each board using three main rules:

Heuristic	Meaning
Monotonicity	Keeps tiles in a snake-like pattern
Smoothness	Penalizes large jumps between tiles
Empty Cells	Rewards open spaces for survival
🔹 3. Survival Mode

If the board becomes dangerous:

Normal depth: 4

Danger mode depth: 6

This helps the AI escape losing positions.

📂 Live Demo

(Replace with your GitHub Pages link)
👉 Play the Game

🛠️ Setup
Clone the Repo
git clone https://github.com/jacklim-gif/2048-With-AI-Auto-Solve.git

Run it

Just double-click:

game.html


No build. No dependencies.

⚙️ Configure the AI
const CONFIG = {
    size: 4,
    aiDelay: 150,
    aiDepth: 4,
    survivalDepth: 6
};

🤝 Contributing
Fork → Branch → Commit → Push → PR

📜 License

MIT License — Free to use & modify.

<div align="center">
💙 Built with passion by Jack Lim

If you want, I can also design:
✔ A custom banner
✔ Preview GIF
✔ Better layout with icons
✔ Color theme for the README

Just say the word.

</div>
