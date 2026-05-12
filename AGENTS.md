# AGENTS.md

## Cursor Cloud specific instructions

This is a minimal static HTML project (image carousel). There is no build system, no package manager, and no backend.

### Running the dev server

Serve the project with Python's built-in HTTP server:

```
python3 -m http.server 8080 --directory /workspace
```

Then open `http://localhost:8080/` in a browser.

### Key notes

- There are no linting, testing, or build tools configured. The project is a single `index.html` with inline CSS/JS.
- The `styles.css` referenced in `index.html` does not exist in the repo; all critical styles are inlined in a `<style>` tag.
- Carousel images are in the `image/` directory (`1.jpg`, `2.jpg`, `3.jpg`).
- No dependencies need to be installed — zero `package.json`, `requirements.txt`, or similar files.
