# Rock Paper Scissors - Data Structures Edition

This is a terminal-based Rock, Paper, Scissors game written in Python that emphasizes the use of data structures for flexibility and customization.

---

## 🎯 Project Purpose

This game is built to help developers understand Python dictionaries, file I/O, and modular programming, all while enjoying a fun and customizable game.

---

## 🧰 Requirements

- macOS Terminal (preferred)
- Python **3.10+**
- Recommended: Virtual environment

---

## ⚙️ Setup Instructions (macOS)

### 1. Clone or download this repository.

### 2. Open Terminal and navigate to the project folder:

```bash
cd path/to/project-folder
```

### 3. Create and activate a virtual environment:

```bash
python3 -m venv venv
source .venv/bin/activate
```

### 4. Install dependencies:

```bash
pip install -r requirements.txt
```

If `requirements.txt` doesn’t exist, install manually:

```bash
pip install colorama prompt_toolkit
```

---

## 🚀 Running the Game

Use the terminal to run the game (recommended for full color support via `colorama`):

```bash
python rpsgame.py
```

---

## 📁 File Overview

| File             | Description                                 |
|------------------|---------------------------------------------|
| `rpsgame.py`     | Main game logic                             |
| `rolls.json`     | Defines valid moves and win/loss rules      |
| `leaderboard.json` | Stores win counts across sessions         |
| `rps.json`       | Log file that tracks in-game events         |

---

## 🪄 Customization

### 🔁 Add New Moves

You can expand the game by modifying `rolls.json`. Example:

```json
{
  "rock": {
    "defeats": ["scissors", "lizard"],
    "defeated_by": ["paper", "spock"]
  },
  "spock": {
    "defeats": ["scissors", "rock"],
    "defeated_by": ["paper", "lizard"]
  }
}
```

Just follow the structure: each move should list what it `defeats` and what it is `defeated_by`.

---

## 🔄 Reset the Leaderboard

To reset the leaderboard, delete the `leaderboard.json` file:

```bash
rm leaderboard.json
```

The file will be recreated the next time a game is played.

---

## 🐞 Troubleshooting

- If autocomplete doesn't work, you're probably running from PyCharm. Run from Terminal instead.
- If `colorama` colors don't display properly, try a different terminal emulator like iTerm2.

---

## 📜 License

This project is for educational and recreational use.
