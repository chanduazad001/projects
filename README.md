# projects

Project portfolio hub — links out to individual project repos, grouped by
category, published as a GitHub Pages project site.

**Published site:** https://chanduazad001.github.io/projects/

## Structure

Plain static HTML, no build step, no framework:

- `index.html` — landing page, links into each category
- `python.html`, `cloud.html`, `devsecops.html`, `ai.html` — one portfolio
  page per category, each a grid of cards
- `style.css` — shared styling across all pages

Each project is its own repo, published independently (its own GitHub Pages
site if applicable). This repo only indexes them.

To add a project: build/publish the project's own repo first, then add one
`.project-card` to the relevant category page here, replacing or alongside
the `.project-card.placeholder` card.

## Publishing

No GitHub Actions workflow needed — GitHub Pages serves these files directly
from the `master` branch root once **Settings → Pages → Source** is set to
"Deploy from a branch" / `master` / `/ (root)`. `.nojekyll` disables the
default Jekyll processing step since this is plain HTML.

## License

See [LICENSE](LICENSE).
