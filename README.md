# Hugo Kuznicki — Personal Site

My personal brand / portfolio site and central content home. It's where my
social profiles point, and where I show the AI-automation and trading tools
I build in public.

**Live:** https://kuznickicapital-ship-it.github.io/personal-site/

## Stack

Plain static site — no build step.

- `index.html` — all content/markup
- `styles.css` — design system (dark, quant-flavored theme)
- `script.js` — sticky nav, mobile menu, scroll reveals

Fonts via Google Fonts CDN. Everything else is self-contained, so GitHub Pages
serves it directly from the repo root.

## Sections

- **Hero** — name, tagline, value prop, primary CTAs
- **Work** — shipped projects (Market Scanner, Content Studio, Content Dashboard, Apex Wallet)
- **About** — short bio + at-a-glance stack panel
- **Services** — "work with me" packages (placeholder pricing, easy to edit)
- **Contact** — email, LinkedIn, X, GitHub, Upwork/Fiverr placeholders

## Editing

Everything is hand-editable HTML/CSS:

- **Pricing** — search `$X,XXX` in `index.html` and drop in real numbers.
- **Screenshots** — Market Scanner and Content Studio pull live screenshots
  from their repos. Content Dashboard / Apex Wallet show `[SCREENSHOT]` /
  `[CASE STUDY]` placeholders; add an `<img>` to those `.card__shot` blocks
  to replace them.
- **Links** — confirm/replace the LinkedIn URL and add Upwork/Fiverr URLs in
  the Contact section.
- **Colors** — tweak the CSS variables at the top of `styles.css`.

## Local preview

Just open `index.html` in a browser, or:

```bash
python -m http.server 8080
# then visit http://localhost:8080
```

## Deploy

Pushing to `main` auto-publishes via GitHub Pages (source: `main` / root).

## Custom domain

To use a custom domain, add a `CNAME` file at the repo root containing the
domain, then set the DNS records GitHub shows under Settings → Pages.
