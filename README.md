# Personal website — Zhongxuan Li

Single-page static site, no build step. Lives at `https://laurelli7.github.io`.

```
index.html   Everything: about, publications, teaching, awards
style.css    All styling (colors and sizes in the :root block)
```

Every push to `main` republishes the site within a minute or two.

## Filling in the placeholders

HTML comments in `index.html` mark each spot:

- **Photo** — drop `profile.jpg` in the repo root and swap the initials `<div class="avatar">` for the `<img>` tag shown in the comment above it.
- **Scholar link** — replace `YOUR-ID` in the sidebar with your Google Scholar profile ID, or delete that list item.
- **Resume** — the sidebar links to `cv.pdf`. Add the file or remove the link.
- **Dates** — the Teaching entry says `Term`, the two award entries say `Year`.
- **Teaching duties and award details** — both are described generically; edit to match reality.

## Editing notes

- Sections are `<section id="...">` blocks in `index.html`; the top navbar links to them by anchor. Add or remove a section and its navbar link together.
- Light/dark mode is a toggle in the navbar (gear position, sun/moon icon). It follows the visitor's system preference by default and remembers their choice in localStorage.
- Colors live in the `:root` (light) and `[data-theme="dark"]` blocks at the top of `style.css`.
