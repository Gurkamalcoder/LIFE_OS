# LIFEOS-ready(UI)

A personal life-tracking toolkit with both a console-based game-like interface and a Flask backend. It uses JSON storage for player state, quests, phase progress, and session logs.

## Features

- Console interface via `main.py`
- Flask backend via `server.py`
- Persistent storage in `app/storage/`
- Colorized terminal output using `colorama`
- Session and phase tracking for daily progress

## Requirements

- Python 3.12+ (project files reference Python 3.12)
- `Flask`
- `colorama`

Install dependencies with:

```bash
pip install -r requirements.txt
```

## Usage

Run the console interface:

```bash
python main.py
```

Run the backend server:

```bash
python server.py
```

Then open `http://localhost:5000` in your browser.

## Project structure

- `main.py` — console app entrypoint
- `server.py` — Flask backend and API layer
- `app/core/` — core app logic, including player, quests, stats, and phase tracking
- `app/storage/` — JSON data files and session logs

## Notes

- The project stores runtime data in `app/storage/`
- Ignore `venv/`, `__pycache__/`, and storage files with `.gitignore`
