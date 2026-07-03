# AGENTS.md

## Cursor Cloud specific instructions

This repository is a **fully static HTML resume site** (no build step, no package
manager, no server-side code). Content lives in a few standalone files:

- `index.html` — print/PDF-oriented resume (two-column dark sidebar layout).
- `web.html` — responsive web version of the resume.
- `photo.jpg`, `assets/` — images referenced by the pages.

### Running the site (development)

There is nothing to install or build. Serve the repo root with any static file
server and open the pages in a browser, e.g.:

```bash
python3 -m http.server 8000
# then open http://localhost:8000/index.html or http://localhost:8000/web.html
```

### Non-obvious notes

- Tailwind CSS, Google Fonts (Inter / Noto Sans SC), and Font Awesome are loaded
  from **CDNs at runtime**. The pages need outbound network access to render with
  full styling; offline, the HTML will still load but appear unstyled.
- There are **no automated tests, linters, or build commands** in this repo.
  Verification is purely visual (open the pages in a browser).
- PDF export is done manually via headless Chrome (see `README.md`); it is not
  part of any automated workflow.
