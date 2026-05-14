# aishwarya — portfolio

Playful, colorful personal portfolio. Single-file static site, hosted on GitHub Pages.

## Stack

- Plain HTML + CSS (no framework, no build step)
- Fonts: Instrument Serif + Plus Jakarta Sans + JetBrains Mono (Google Fonts)
- One file: `index.html`

## Before you publish — TODO

Open `index.html` and update the contact section (search for `your.email`, `your-handle`):

1. Email — replace `your.email@example.com`
2. LinkedIn handle — replace `@your-handle`
3. GitHub handle — replace `@your-handle`

Optional: drop `resume.pdf` in the repo root.

## See it locally

Just double-click `index.html` — it opens in your browser. Or run a quick local server:

```bash
python3 -m http.server 8000
# then open http://localhost:8000
```

## Deploy to GitHub Pages

### Option A — `<username>.github.io` (clean URL)

```bash
# 1. Create a GitHub repo named exactly: <your-username>.github.io
git init
git add .
git commit -m "initial portfolio"
git branch -M main
git remote add origin https://github.com/<your-username>/<your-username>.github.io.git
git push -u origin main
```

Live at `https://<your-username>.github.io` in ~1 minute.

### Option B — any repo name

```bash
git init
git add .
git commit -m "initial portfolio"
git branch -M main
git remote add origin https://github.com/<your-username>/portfolio.git
git push -u origin main
```

Then on GitHub: **Settings → Pages → Source: `main` / root → Save**.
Lives at `https://<your-username>.github.io/portfolio/`.

## Customizing colors

All colors are CSS variables at the top of `index.html` under `:root`. Swap `--coral`, `--pink`, `--violet`, `--yellow` etc. to retheme without touching anything else.
