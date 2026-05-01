# CURA Branding Repository

## What this repo is

Canonical brand identity kit for CURA — an AI automation consultancy for SMEs. Published as a GitHub Pages site (`index.html`) and consumed by AI agents, partners, and internal tools via `brand-identity.json`.

## Key files

| File | Purpose |
|---|---|
| `brand-identity.json` | Single source of truth — all brand tokens, colors, typography, voice, UI patterns |
| `BRAND.md` | Human-readable brand guide (mirrors the JSON in prose) |
| `index.html` | GitHub Pages brand kit SPA — the visual representation of the brand |
| `cura-logo-dark-Bjrh0FR_.webp` | Official logo — 3D metallic blue CA monogram with wordmark |
| `LICENSE.md` | All rights reserved, CURA |

## GitHub Pages

The site is served from `index.html` at the repo root on the `main` branch. No build step — pure HTML/CSS/JS, zero external dependencies except Google Fonts (Inter, JetBrains Mono loaded via `<link>`).

To deploy: commit changes to `main`. GitHub Pages picks up `index.html` automatically.

## Brand constraints for AI agents

When generating any content for or about CURA, consult `brand-identity.json`. Key rules:

- **Dark-first** — primary background is `#080C14`, never use light backgrounds in the platform UI
- **Primary accent** is `#3B82F6` (blue), secondary is `#14B8A6` (teal)
- **Font** — Inter for all UI; JetBrains Mono for code/data
- **Logo** — always use `cura-logo-dark-Bjrh0FR_.webp`; never stretch or recolor; maintain clear space equal to icon height on all sides
- **Voice** — results-led, concrete numbers, no hype language ("revolutionary", "game-changing")
- **Key phrases** — "AI Automation, Done Right" · "Real Results, Proven ROI" · "Your Data, Protected" · "Up to 6 hours saved per day"

## index.html conventions

- All brand tokens are CSS custom properties on `:root`; light mode overrides live under `[data-theme="light"]`
- Theme toggle (sun/moon) in the nav persists to `localStorage` under key `cura-theme`; respects `prefers-color-scheme` on first visit; set via inline `<script>` in `<head>` before CSS to prevent flash
- Color swatches are click-to-copy (hex copied to clipboard via `copyHex()`)
- Sections: Hero → Logo → Colors → Typography → Gradients → Components → Voice → Tokens → Footer
- Colors section has three dividers: Dark Mode tokens · Light Mode tokens · Shared (accent, semantic, chart)
- No frameworks, no build tools — edit the single file directly
- When adding new brand tokens, update `brand-identity.json` first, then reflect the CSS vars in `index.html`
- Shadows, gradients, and grid lines all have light mode overrides — check `[data-theme="light"]` block when editing
