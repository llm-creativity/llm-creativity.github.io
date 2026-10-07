# Getting It Right, Under Constraint — project page

Static project page for *Getting It Right, Under Constraint: Evaluating and Improving LLM Creativity*.

The whole site is a single file, `index.html`. Fonts are loaded from Google Fonts; all images are embedded in the file, so nothing else needs to be hosted.

## Status

**Not live yet.** The repository is private and GitHub Pages is not enabled, so nothing is served.

## Preview locally

Open `index.html` in a browser, or run a small server from the repo root:

```
python3 -m http.server 8000
```

Then visit http://localhost:8000.

## Before going live

Edit `index.html`:

- Put the real arXiv URL and code-repository URL into the two `href="#"` links in the `<nav class="links">` block near the top.
- Check the BibTeX entry in the `#citation` section.

## Going live (GitHub Pages)

This repository is the organization site for `llm-creativity`, so once it is public
GitHub Pages serves it automatically from the root of `main`.

1. Make sure everything is on `main`.
2. GitHub Pages on a free plan only works for **public** repositories. When you are ready, make
   the repository public: Settings → General → Danger Zone → Change visibility.
3. GitHub enables Pages on its own for a repository named `<org>.github.io`. If it does not,
   go to Settings → Pages → Build and deployment → Source: **Deploy from a branch** →
   Branch: `main`, folder `/ (root)` → Save.
4. After a minute or two the site is served at `https://llm-creativity.github.io/`.

Note: making the repository public is the same moment the site goes live.

The `.nojekyll` file tells GitHub Pages to serve the files exactly as they are, without running Jekyll.

To take the site down again, set Settings → Pages → Source back to **None**.
