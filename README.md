# xwave40.com

Website and brand files for **xWave40 LLP** — *AI-Powered Software*.

## What's in this repo

| Path | What it is |
|---|---|
| `site/` | The website. This folder is what gets published. |
| `site/index.html` | The whole site: HTML, CSS and JavaScript in one file. |
| `site/assets/` | Logo, link-preview image and app icon used by the site. |
| `brand-kit/` | Logo, icon, visiting card, letterhead and colour files (not published). |
| `netlify.toml` | Tells Netlify to publish the `site/` folder. |
| `CLAUDE.md` | Notes for Claude when editing this project. |

## Preview locally

Open `site/index.html` in a browser, or run a small local server:

```bash
npx serve site
```

Then open the address it prints (usually http://localhost:3000).

## Deploy on Netlify

1. In Netlify, choose **Add new site → Import an existing project → GitHub**, and pick this repo.
2. Netlify reads `netlify.toml`, so there is nothing to configure. Click **Deploy**.
3. Under **Domain management**, add `xwave40.com` and add the DNS records Netlify shows at your domain provider (Squarespace).

After that, every push to `main` updates the live site automatically.

The contact form uses Netlify Forms; submissions appear in Netlify under **Forms**.

## Brand at a glance

- Logo: `site/assets/logo-on-white.svg` and `logo-on-navy.svg`
- Tagline: AI-Powered Software
- Fonts: Lexend Exa (brand), Barlow Semi Condensed (headings), Barlow (body)
- Colours: Card Navy `#0F1E3A`, Deep Space Navy `#070B14`, Signal Blue `#1F6FD1`, Horizon Blue `#4AA8FF`, Slate Grey `#5C626D`, White `#FFFFFF`
