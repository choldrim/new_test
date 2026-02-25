# AGENTS.md

## Cursor Cloud specific instructions

This is a zero-dependency, single-file browser game (消消乐 / Match-3 puzzle). The entire application lives in `index.html` — no build step, no package manager, no tests.

### Running the application

Serve the project root with any static HTTP server:

```
python3 -m http.server 8080
```

Then open `http://localhost:8080/index.html` in a browser.

### Lint / Test / Build

- **Lint**: No linter is configured. For ad-hoc HTML/JS validation, use an external tool (e.g. `npx htmlhint index.html`).
- **Tests**: No automated test suite exists.
- **Build**: No build step — the file is served as-is.

### Notes

- The game is entirely client-side JavaScript (vanilla ES6+, no frameworks).
- All CSS is inlined in `<style>` and all JS is inlined in `<script>` within `index.html`.
- No environment variables or secrets are required.
