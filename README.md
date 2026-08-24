# Personal website — Zhongxuan Li

Static site, no build step. Five pages sharing one stylesheet.

```
index.html          About
publications.html   Papers + other contributions
teaching.html       Teaching
awards.html         Honors & fellowships
misc.html           Miscellaneous
style.css           All styling
```

## Put it on GitHub Pages

Your site will live at `https://Laurelli7.github.io`.

1. On GitHub, create a **new public repository** named exactly `Laurelli7.github.io`. Leave it empty (no README, no .gitignore).
2. Put these files in the repository root. `index.html` must be at the top level, not in a subfolder.

   ```bash
   git init
   git add .
   git commit -m "Add personal site"
   git branch -M main
   git remote add origin https://github.com/Laurelli7/Laurelli7.github.io.git
   git push -u origin main
   ```

   Or use the web UI: **Add file → Upload files**, drag all six files in, commit.
3. Go to **Settings → Pages**. Under "Build and deployment", set Source to **Deploy from a branch**, branch `main`, folder `/ (root)`. Save.
4. Wait a minute or two, then open `https://Laurelli7.github.io`.

Every push to `main` republishes the site.

### Repository named something else

If the repo isn't `Laurelli7.github.io`, the site publishes at `https://Laurelli7.github.io/<repo-name>/` instead. Everything still works — all links between pages are relative.

## Before you publish

A few placeholders need your real values. Search for `YOUR-ID` across the HTML files:

- **Scholar link** — the sidebar of all five pages, and again at the bottom of `misc.html`, points to `YOUR-ID`. Replace it with your Google Scholar profile ID, or delete the link if you don't have a profile yet. (GitHub already points to `Laurelli7`.)
- **CV** — the sidebar links to `cv.pdf`. Drop that file in the repo root, or remove the link.
- **Dates** — `teaching.html` says `Term` and `awards.html` says `Year`. Replace with the actual quarter and years.
- **Award details** — I described both awards generically since I didn't want to invent specifics. Add the awarding body for the T. D. Lee Fellowship and a line about what the Quad Scholar funding supported.
- **Teaching duties** — the Understanding AI entry describes typical TA work. Edit it to match what you actually did.
- **Miscellaneous** — that page is scaffolding with three prompts. Replace them or delete the page (and its nav link in the other four files).

HTML comments mark each of these spots inline.

## Editing notes

The navigation appears in all five files. If you add or rename a page, update the `<nav class="cfg">` block in each one.

The current page is marked with `aria-current="page"` on its `<li>`, which is what fills in the indigo dot on the nav spine. Keep that attribute on exactly one item per page.

Colors and spacing live in the `:root` block at the top of `style.css`.
