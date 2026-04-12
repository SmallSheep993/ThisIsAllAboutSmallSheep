# This Is All About SmallSheep

Personal portfolio site for **Alex Yang (SmallSheep)** — Rutgers Computer Science student. Static pages for projects, interests, a movie list, and contact links.

**Live site:** [https://smallsheep993.github.io/ThisIsAllAboutSmallSheep/](https://smallsheep993.github.io/ThisIsAllAboutSmallSheep/)

## Pages

| Page | File | Description |
|------|------|-------------|
| Home | `index.html` | Intro, profile-style code panel, current plans, embedded [Jumper](https://smallsheep993.github.io/A-Jumper-Game/) game, contact |
| Projects | `projects.html` | Technical project cards with GitHub links |
| Things I like | `things.html` | Hub linking to interest subpages |
| Movie list | `movies.html` | Favorites and watchlist with local poster images |
| Interests | `interests/*.html` | Climbing, fitness, food, hiking, travel |

## Tech stack

- **HTML5** — semantic structure, multi-page layout
- **CSS** — shared stylesheet `site.css` (Outfit + JetBrains Mono via Google Fonts)
- **JavaScript** — minimal; `script.js` sets the footer year; the home page uses inline `IntersectionObserver` for scroll-in animations

No build step or framework — deploy as static files.

## Local preview

From the repository root, serve the folder over HTTP (any static server works). Examples:

```bash
python3 -m http.server 8080
# Open http://localhost:8080
```

```bash
npx --yes serve .
```

Opening `index.html` directly in a browser works for a quick look; a local server avoids oddities with paths and caching when testing all pages.

## Project layout

```
├── index.html
├── projects.html
├── things.html
├── movies.html
├── script.js
├── site.css
├── style.css              # legacy / unused — all pages link to site.css
├── assets/
│   └── images/            # movie posters; see Assets note below
├── interests/
│   ├── climbing.html
│   ├── fitness.html
│   ├── food.html
│   ├── hiking.html
│   └── travel.html
├── README.md
└── .gitignore
```

## Deployment (GitHub Pages)

Host from the repository’s default branch using **GitHub Pages** (site root or your configured publish directory). After you push, allow a short time for the live site to update.

If your GitHub repository name differs from this local folder, set **Settings → Pages** to match that repo’s published URL.

## Assets note

`index.html` references `assets/images/profile.jpg` for the contact section. Add that file under `assets/images/` if you want the avatar to show on the deployed site.

## Author

**Alex Yang** · SmallSheep — contact and social links are on the [home page](https://smallsheep993.github.io/ThisIsAllAboutSmallSheep/) contact section.

## License

No license file is bundled by default. Add a `LICENSE` (for example MIT) if you want to specify terms for this site’s source code.
