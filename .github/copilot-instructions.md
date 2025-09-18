# Copilot Instructions — Javascript-AI-Assisted-Coding

These instructions orient an AI coding agent for quick, accurate contributions to this small repository.

Goal
- Make minimal, correct edits that preserve the repository's simple structure and HTML-first intent.

What this project contains
- Single-page example: `Javascript-AI-Assisted-Coding.html` — a plain HTML file with an inline `<script>`.
- Minimal `README.md` with only a title.

High-level guidance for edits
- Keep changes minimal and focused: this repo is a single-file demo. Avoid adding complex build tooling or new folders unless asked.
- Preserve file encoding and simple HTML formatting.
- Prefer browser-compatible, standards-based fixes (vanilla JS) rather than adding packages.

Common patterns and concrete examples
- DOM access: follow correct DOM API names and casing. Example bug in `Javascript-AI-Assisted-Coding.html`: `document.GetElementById("demo")` should be `document.getElementById("demo")` (lowercase `g`).
- Ensure referenced DOM elements exist before writing to them. If adding content, either add the target element in the HTML or guard writes with a null-check.

Example quick-fix recipe (apply when appropriate)
- If script references a missing element id `demo`:
  - Option A (add element): add `<div id="demo"></div>` to the page body near the script.
  - Option B (guard): change script to `const el = document.getElementById('demo'); if (el) el.innerHTML = 'Hello World!';`.

Developer workflows (what an agent should assume)
- No build or test commands present — changes are validated by opening the HTML in a browser.
- For code quality, prefer minimal lint-style fixes (correct API names, casing, missing semicolons) within the single file.

Integration points and external dependencies
- None detected. Do not add external CDN dependencies without explicit user instruction.

When to create new files or expand the project
- Ask the user before adding: package manifests (`package.json`), scaffolding, or CI configs. This repo appears intentionally minimal.

Commit message guidance
- Keep commits focused and atomic. Use messages like: `fix(html): correct getElementById casing and guard DOM write` or `chore: add demo element to HTML`.

If unsure
- Ask the repository owner whether they want the repository to stay minimal or be expanded into a demo project with build tooling.

References (files to inspect when working)
- `Javascript-AI-Assisted-Coding.html` — main file to edit for examples and fixes.
- `README.md` — minimal project description.

End of instructions. Reply with suggested change before applying for non-trivial edits.
