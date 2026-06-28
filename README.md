# Personal landing page

A static, single-page site to share my work and talks — hosted free on GitHub Pages.
First feature: my Call for Presentations submission for **C-Days 2026** (CNCS).

## Structure

```
.
├── index.html        # the page (edit text + cards here)
├── css/
│   └── style.css     # dark / cyber theme
├── assets/
│   ├── c-days-2026.pdf   # ← drop your PDF here (see assets/README.txt)
│   └── favicon.svg
├── .nojekyll         # tells GitHub Pages to serve files as-is
└── README.md
```

## Before you publish — replace the placeholders

In `index.html`:
- `YOUR NAME` → your name
- the tagline / about / card text
- `YOUR-USERNAME` → your GitHub username (GitHub + og:url links)
- `you@example.com` and the LinkedIn URL

Then put your PDF at `assets/c-days-2026.pdf`.

## Deploy to GitHub Pages

**Option A — user site (URL: `https://YOUR-USERNAME.github.io`)**
1. Create a repo named exactly `YOUR-USERNAME.github.io`.
2. Upload everything in this folder to the repo root (keep the folders).
3. Repo → **Settings → Pages** → Source: **Deploy from a branch** → Branch: `main` / `/ (root)` → Save.
4. Wait ~1 minute, then visit `https://YOUR-USERNAME.github.io`.

**Option B — project site (URL: `https://YOUR-USERNAME.github.io/REPO-NAME`)**
1. Create any repo (e.g. `landing`), upload these files.
2. Same Pages setting as above. URL becomes `https://YOUR-USERNAME.github.io/landing`.

### Upload via the website (no git needed)
Repo page → **Add file → Upload files** → drag the contents of this folder in → **Commit**.

### Or via command line
```bash
git init
git add .
git commit -m "Landing page + C-Days 2026"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/YOUR-USERNAME.github.io.git
git push -u origin main
```

## Adding more talks later
Duplicate a `<article class="card">…</article>` block in `index.html`, drop the new
PDF/slides in `assets/`, and link them. No build step — just edit and push.
