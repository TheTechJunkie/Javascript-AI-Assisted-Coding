# Javascript-AI-Assisted-Coding

This repository is a tiny single-file demo: `Javascript-AI-Assisted-Coding.html` — a minimal HTML + Canvas platformer implemented with vanilla JavaScript.

Play / Run instructions

- Open the file directly in a browser: double-click `Javascript-AI-Assisted-Coding.html` or use your browser's "Open File" command.
- Alternatively, serve the folder locally (recommended for consistent behaviour) and open `http://localhost:8000/Javascript-AI-Assisted-Coding.html`:

```bash
# from the repository root
python3 -m http.server 8000
# then open http://localhost:8000/Javascript-AI-Assisted-Coding.html
# Javascript-AI-Assisted-Coding

This repository is a tiny single-file demo: `Javascript-AI-Assisted-Coding.html` — an HTML + Canvas platformer implemented with vanilla JavaScript.

Features added

- Multiple levels with a simple level selector (`Prev Level` / `Next Level`).
- Collectible items that grant score.
- Patrolling enemies that cost a life on contact.
- Score, Lives, and Level HUD.
- Smooth camera with lookahead and a simple parallax background.
- Gamepad support (standard controllers); no touch controls — keyboard or controller only.

Play / Run instructions

- Open the file directly in a browser: double-click `Javascript-AI-Assisted-Coding.html` or use your browser's "Open File" command.
- Alternatively, serve the folder locally and open `http://localhost:8000/Javascript-AI-Assisted-Coding.html`:

```bash
# from the repository root
python3 -m http.server 8000
# then open http://localhost:8000/Javascript-AI-Assisted-Coding.html
```

Controls

- Move: Left / Right arrow or A / D
- Jump: Up arrow, W, or Space
- Restart: Click the "Restart" button
- Level: `Prev Level` / `Next Level` buttons in the page
- Gamepad: Axis 0 for left/right, button 0 for jump (A / Cross)

Notes for contributors / AI agents

- Keep edits minimal and HTML-first — this repo is intentionally small.
- Prefer vanilla JS fixes; avoid adding new packages or build tooling unless the owner requests expansion.

If you'd like further features (mobile controls removed per request), suggest one area (visuals, more enemies, level editor, or GitHub Pages deploy) and I will implement it.