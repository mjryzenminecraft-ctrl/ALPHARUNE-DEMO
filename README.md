# ALPHARUNE: DEMO Title 1 (Title 1 Beta coming out soon)

**ALPHARUNE: Title 1** is an open-source, sci-fi RPG tribute built in Python using Pygame, heavily inspired by Toby Fox's *Deltarune* and *Undertale*. 

The game mirrors the classic shift from a peaceful Overworld to surreal alternate realms. Players control the **Alpha Group**—Orion, Vexa, and Proto—as they travel through glitching Core Dimensions to seal unstable **Alphalites Cores** before their reality collapses.

---

## 🎮 Core Mechanics & Features

*   **The Sync-Grid Battle System:** A high-tech twist on traditional turn-based bullet-hell combat. Dodge incoming projectiles inside a shifting matrix; stepping on glowing data tiles charges your team's abilities faster.
*   **The Power of Choice:** True to its inspirations, combat is a choice. You can physically smash glitches using Vexa's Plasma Gauntlet, or use Orion and Proto's actions to peacefully "De-frag" and rewrite corrupted code.
*   **JSON-Powered Persistence:** Player progress, choices, inventory, and stats are dynamically handled using an external `alpharune_save.json` architecture.

---

## 🛠️ Developer Setup & Code Execution

If you are a developer interested in exploring the source code or contributing to the project, follow these steps to run the game from source:

### Prerequisites
Make sure you have **Python 3.x** installed on your system. 

### 1. Clone the Repository
```bash
git clone https://github.com
cd ALPHARUNE-Title-1
```

### 2. Install Dependencies
This project relies on the **Pygame** library for graphic rendering, window management, and input loops:
```bash
pip install pygame
```

### 3. Run the Game
Execute the main entry point script to launch the window loop:
```bash
python alpharune.py
```

---

## 📦 How We Build the Standalone Executable (`.exe`)

For regular players, the project is compiled into a standalone application so they can play without downloading Python or Pygame. If you want to bundle your changes into a fresh executable, we use **PyInstaller**:

```bash
pip install pyinstaller
python -m PyInstaller --onefile --windowed alpharune.py
```

### Important Directory Structure for Release
After compilation, ensure your `dist/` release folder architecture matches this layout so that the executable can locate asset resources and read/write the local state:

```text
dist/
├── alpharune.exe             # Compiled binary application
├── alpharune_save.json       # Game state configuration database
└── assets/                   # Textures, sprites, fonts, and sound cues
```

---

## 🤝 Contributing & Support
Contributions, bug reports, and asset suggestions are highly welcome! 
1. Fork the Project.
2. Create your Feature Branch (`git checkout -b feature/AlphaMechanic`).
3. Commit your Changes (`git commit -m 'Add some AlphaMechanic'`).
4. Push to the Branch (`git push origin feature/AlphaMechanic`).
5. Open a Pull Request.

*Disclaimer: This is a fan-developed indie game created out of absolute admiration for Deltarune. All rights to the original formulas belong to Toby Fox.*
