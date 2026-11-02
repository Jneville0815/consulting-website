# consulting-website

Jimmy's AI consulting site for https://jimmyneville.com, served by GitHub Pages
from `main`. One page of plain HTML, one CSS file, and a small inline script
for scroll reveals. There is no build step.

@~/Projects/project-core/REPO.md

## Map

Every tracked path in this repo.

| Path | Holds |
| --- | --- |
| `.claude/settings.json` | Hook wiring. Which shared script runs on which event |
| `.claude/skills/` | This repo's own skills, and one symlink per shared skill in project-core |
| `CLAUDE.md` | This file. What the repo is, its guardrails, and this Map |
| `CNAME` | The custom domain GitHub Pages serves. Do not remove it |
| `MEMORY.md` | The Memory queue: proposed changes, drained by `/review-memory` |
| `README.md` | How to preview the site locally |
| `_config.yml` | Keeps `CLAUDE.md`, `MEMORY.md`, and `README.md` off the published site |
| `favicon.svg` | The tab icon: a cream J on green with an amber dot |
| `img/` | Site images. `jimmy.jpg` is the About photo, cropped to 4:5 with its location data stripped. `og.png` is the 1200x630 link preview image |
| `index.html` | The whole site |
| `style.css` | All styles. Colors and fonts are tokens on `:root` |

## Guardrails

- Once the repo has a GitHub remote, `land-main.sh` pushes every turn, and a
  push to `main` publishes the site.
- Keep the copy minimal and plain. Draft any new copy with `write-for-humans`.
- Never name the technologies, platforms, or vendors behind client work
  anywhere on the site.
- Strip location data from any photo before adding it to `img/`.
