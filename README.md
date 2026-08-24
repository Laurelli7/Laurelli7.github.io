# Personal website — Zhongxuan Li

Single-page static site, no build step. Lives at `https://laurelli7.github.io`.

```
index.html   Everything: about, publications, teaching, awards
style.css    All styling (colors and sizes in the :root block)
```

Every push to `main` republishes the site within a minute or two.

## Filling in the placeholders

HTML comments in `index.html` mark each spot:

- **Scholar link** — replace `YOUR-ID` in the sidebar with your Google Scholar profile ID, or delete that list item.
- **Resume** — the sidebar links to `cv.pdf`. Add the file or remove the link.
- **Teaching duties and award details** — both are described generically; edit to match reality.

## Editing notes

- Sections are `<section id="...">` blocks in `index.html`; the top navbar links to them by anchor. Add or remove a section and its navbar link together.
- Colors live in the `:root` block at the top of `style.css`.
