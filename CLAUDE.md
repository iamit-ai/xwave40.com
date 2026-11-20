# xwave40.com — notes for Claude

Company website for xWave40 LLP (Pune · Kolhapur · USA). Tagline: **AI-Powered Software**.
Services: E-Governance, Artificial Intelligence, Legal Compliance, Product Development, Automation.
Product featured on the site: xarathi.ai (free court-case tracker on official eCourts records; English, Marathi, Hindi).

## Structure

- `site/index.html` is the entire website: one self-contained file with inline CSS and JS. No framework, no build step.
- `site/assets/` holds images the page links to (`/assets/...`). Keep paths absolute from the site root.
- `brand-kit/` is reference material (logos, card, letterhead, colours). It is not published; don't link to it from the site.
- Netlify publishes `site/` (see `netlify.toml`).

## Conventions

- Keep it a single HTML file unless there's a strong reason to split.
- Style through the CSS custom properties in `:root` (`--bg`, `--panel`, `--glow`, `--signal`, `--muted`, `--font-*`). Don't hard-code new colours.
- Brand colours: Card Navy `#0F1E3A` (panels, footer), Deep Space Navy `#070B14` (page background), Signal Blue `#1F6FD1` (blue on white), Horizon Blue `#4AA8FF` (blue on navy), Slate Grey `#5C626D`, White.
- Fonts (Google Fonts): Lexend Exa for brand/tagline/kickers, Barlow Semi Condensed for headings, Barlow for body.
- The logo is inline SVG in the header and footer, copied from `site/assets/logo-on-navy.svg`. If the logo changes, update both places.
- Write the company name as **xWave40** in body copy; the domain stays lowercase `xwave40.com`.
- The two canvas animations (hero network + planet horizon, and the "We connect the dots" services diagram) must respect `prefers-reduced-motion`; keep that check when editing them.
- The contact form posts to Netlify Forms (`data-netlify="true"`); keep the hidden `form-name` input and the honeypot.
- The xarathi.ai demo's Marathi and Hindi strings live in the `L` object in the script; keep translations accurate.
- Contact details: +91 90285 08787, amit@xwave40.com, LLPIN ACR-9336.

## Checking changes

Preview with `npx serve site` and check both a desktop width and a phone width (~390px).
