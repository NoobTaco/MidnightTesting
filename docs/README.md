# Docs folder

This folder contains the static site for the project (GitHub Pages). A few notes to keep things consistent:

- Canonical images location: `docs/images/` — all site pages and repository Markdown should reference images using `docs/images/<filename>`.
- Why: GitHub Pages is configured to serve the `docs/` folder. Keeping images inside `docs/` means the site will find them reliably and there is a single source of truth.
- How to add images:
  1. Place the image file in `docs/images/`.
 2. Reference it from Markdown or HTML using `docs/images/<filename>` (for repo Markdown) or `images/<filename>` when referenced from files inside `docs/` (because `docs/` is the site root).
 3. Commit and push: `git add docs/images/<filename> && git commit -m "Add image: <filename>" && git push`.

- Notes on paths:
  - For files rendered from the `docs/` folder (e.g., `docs/index.html`), use `images/<filename>` because the site root is `docs/`.
  - For Markdown files in the repository root or other folders, use `docs/images/<filename>` so those files on GitHub point at the same image files that Pages serves.

- Automation suggestion: If you prefer to keep using `images/` in Markdown, consider adding a small script or GitHub Action to sync `images/` and `docs/images/` automatically. This repository currently uses `docs/images/` as the canonical location.

Thanks — keeping a single images location avoids duplicate files and broken links.
