# UMTA — Undergraduate Mock Trial Association

The website for the Undergraduate Mock Trial Association at the University of Windsor, served at [umta.ca](https://umta.ca).

## What this is

A static, multi-page site. Plain HTML, one shared stylesheet, and a small JavaScript file for the mobile menu and scroll animations. There is **no build step** and no dependencies — Vercel serves the files exactly as they are.

## Pages

| File | Purpose |
| --- | --- |
| `index.html` | Home: seal, partners, season stats, highlights, about |
| `competitions.html` | In-house competitions, out-of-town results, community events |
| `white-papers.html` | Legal papers written by members |
| `resources.html` | Competition final recordings and how-to-moot guides |
| `team.html` | Executive team |
| `join.html` | Applications and contact |

## Shared files

- `styles.css` — the entire design system. Colours and spacing are CSS variables defined in `:root` at the top.
- `script.js` — mobile nav toggle, scroll reveal, footer year.
- `images/` — photos and logos.

Every page carries its own copy of the header, footer, and announcement bar. If you change one, change all six.

## Working on it locally

No install needed. Open `index.html` in a browser, or serve the folder:

```
python -m http.server 5620
```

Then visit `http://localhost:5620`.

## Deploying

Pushing to the production branch triggers an automatic Vercel deployment to umta.ca. Pushing to any other branch produces a preview URL without touching the live site.

## Notes

- Image paths are lowercase `images/`. Vercel serves from Linux, where filename case matters, so keep references exact.
- Partner logos (WizePrep, Red Bull) are used to credit real sponsors. If either sends an official asset pack, swap the files in `images/` rather than editing the markup.
