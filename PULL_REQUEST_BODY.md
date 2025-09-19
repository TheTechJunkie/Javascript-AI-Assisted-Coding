Title: feat(platformer): levels, collectibles, enemies, camera, gamepad support and docs

Summary
- Adds multiple levels with a simple level selector (Prev/Next).
- Adds collectible items that increase score and spawn particle effects.
- Adds patrolling enemies that cause life loss on contact.
- Adds score, lives, and level HUD.
- Adds smooth camera with horizontal/vertical lookahead and a simple parallax background.
- Adds basic Gamepad API support (axis 0 for left/right, button 0 for jump).
- Updates `README.md` and adds `.github/copilot-instructions.md` for contributor/AI guidance.

Files changed
- `Javascript-AI-Assisted-Coding.html` — main game implementation and features.
- `README.md` — updated play/run instructions and feature list.
- `.github/copilot-instructions.md` — repo guidance for AI agents.

Testing steps
1. Serve the repo and open the game:
   ```bash
   python3 -m http.server 8000
   # open http://localhost:8000/Javascript-AI-Assisted-Coding.html
   ```
2. Play with keyboard:
   - Move: ←/→ or A/D
   - Jump: ↑/W/Space
   - Use `Prev Level` / `Next Level` to switch levels.
3. Verify collectibles (gold squares) increase score and spawn particles.
4. Verify enemies patrol their ranges and contacting one reduces lives and spawns red particles.
5. Verify reaching the flag progresses to the next level.
6. Connect a gamepad and press any button — HUD should display "Gamepad: connected" and axis/button movement should work.

Checklist
- [ ] Manual playtest completed on keyboard
- [ ] Manual playtest completed with a controller
- [ ] README reviewed and accurate
- [ ] No touch controls added (project remains keyboard/controller-only)

Notes
- The project is intentionally a single-file demo — no build tooling or external deps were added.
- I can open the PR for you if you install the GitHub CLI (`gh`) or provide a temporary personal access token with `repo` permissions.

Commit trigger: 2025-09-19T00:27:58Z
