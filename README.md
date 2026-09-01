# Aosis — Creative Agency

A one-page site for a creative studio: hero, portfolio, services, "why choose us," stats, pricing, team, and a footer for contact. Two files — plain HTML and CSS, no build step, no dependencies to install.

## Project structure

```
.
├── index.html
└── style/
    └── style.css
```

## Getting it

Clone the repo:

```bash
git clone https://github.com/ali-shker/FrontEnd.git
cd FrontEnd
```

Or just download the ZIP from the green "Code" button on GitHub.

## View it

### Locally

Double-click `index.html`, or right-click → Open with → your browser. The stylesheet is linked with a relative path (`style/style.css`), so keep the two together — split them up and it'll load unstyled.

### Deploy it online

It's static, so any of these take a couple minutes:

| Host | Steps |
|---|---|
| **GitHub Pages** | In this repo, go to Settings → Pages, set the source branch to `main` and folder to `/root`. Live at `ali-shker.github.io/FrontEnd`. |
| **Netlify** | Go to `app.netlify.com`, "Add new site" → "Import an existing project," connect this repo. Auto-deploys on every push. |
| **Vercel** | Same idea at `vercel.com` — "Add New Project," import the repo. |

## What's inside

- **Hero** — asymmetric headline layout with a subtle glow, "Order Now" / "Learn More" pills.
- **Portfolio** — a staggered editorial grid of six cards (Brand Identity, Photography, UI Concepts, Creative Ads, Visual Story, Digital Campaign), each with a distinct CSS-gradient background — no image files to break.
- **Services** — six feature cards (App Development, Graphic Design, Creative Idea, Marketing, Awesome Support, Brand Design), one flipped to a dark background for contrast.
- **Why choose us** — bio copy, a checklist of four points, and an image with pagination dots.
- **Stats bar** — four numbers (clients, awards, coffee, projects) on a dark strip.
- **Pricing** — Basic / Business / Premium plans, with the Business plan inverted to a dark card.
- **Team** — three team cards with grayscale-to-color photo hover.
- **Footer** — contact anchor with a copyright line.

## Tech

Plain HTML and CSS. No frameworks, no build tools, no JavaScript. Fonts (Unbounded, Inter) load from Google Fonts; everything else lives in `style.css`.

## Customizing

- **Text/copy** — edit directly inside the `<section>` blocks in `index.html`.
- **Colors** — change the CSS variables at the top of `style.css` (`--ink`, `--paper`, `--cobalt`, `--coral`, etc.).
- **Portfolio card art** — each card's background is its own CSS rule (`.card-one` through `.card-six`) — tweak the gradients there, or swap in a `background-image` if you'd rather use real photos.
- **Team / about photos** — currently Unsplash placeholders, swap the `src` on the relevant `<img>` tags for your own.
- **Pricing plans** — duplicate a `.price-card` block inside the `#prices` section and edit the name, price, and feature list.

## Notes

- Respects `prefers-reduced-motion` — animations are disabled for users who have that OS setting on.
- Fully responsive down to mobile; nav links scroll horizontally on small screens instead of collapsing into a hamburger menu.
- No analytics, tracking, or external scripts beyond the Google Fonts stylesheet.
- Rough edges: the footer has no real contact form yet, the portfolio ✎/⌕ icons don't link anywhere, and the about/team images are still Unsplash placeholders.
