# AGENTS.md

## Cursor Cloud specific instructions

This is a static HTML/CSS/JS image carousel — no build system, package manager, or framework.

### Running the app

Serve the project root with any static HTTP server:

```bash
cd /workspace && python3 -m http.server 8080
```

Then open `http://localhost:8080` in a browser. The carousel cycles through three images (`image/1.jpg`, `image/2.jpg`, `image/3.jpg`) with a CSS fade transition every 3 seconds.

### Lint / Test / Build

- **No linter, test suite, or build step exists.** Validation is manual: open the page in a browser and confirm all three images appear and the carousel transitions work.
- The HTML file references `styles.css` via `<link>` but no `styles.css` file exists in the repo; the relevant styles are inline in `<style>` tags. This is not a bug — the missing external stylesheet is simply unused.
