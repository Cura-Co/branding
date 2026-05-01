<p align="center">
  <img src="cura-logo-dark-Bjrh0FR_.webp" alt="CURA" width="280" />
</p>

<h3 align="center">Brand Identity & Voice Kit</h3>

<p align="center">
  The canonical reference for how CURA looks, sounds, and presents itself — built for agents, partners, and internal teams.
</p>

---

## What's in this repo

**`brand-identity.json`** — The single source of truth for CURA's brand. Covers:

- **Company** — positioning, tagline, target audience, value proposition, product descriptions, and partner ecosystem
- **Visual identity** — full color system (foundation, text, accent, semantic, chart palettes), gradients, typography scale, spacing tokens, border radii, and shadows
- **Logo** — detailed description of the 3D metallic blue CA monogram, color profile, file references, and usage guidelines
- **UI patterns** — navigation, dashboard cards, stat badges, tables, buttons, charts, and search bar conventions as used across the Command Centre platform
- **Voice & tone** — brand personality, tone guidance by context (marketing, product, support), writing principles, key phrases, and language to avoid
- **Data & metrics** — the KPIs and team metrics surfaced in the Command Centre
- **Security** — CURA's data-protection messaging and commitment

**`cura-logo-dark-Bjrh0FR_.webp`** — Official dark-variant logo (3D metallic blue CA monogram with wordmark).

## Usage

This repo is designed to be consumed by AI agents, automation tools, and partner integrations that need to represent or interact with the CURA brand. Point any system to `brand-identity.json` for structured access to colors, typography, voice guidelines, and more.

```jsonc
// Example: pull the primary accent color
{
  "visual.colors.accent.primary.hex": "#3B82F6"
}
```

## About CURA

CURA is an AI automation consultancy for SMEs and growing businesses. We combine strategic consulting with our proprietary Command Centre platform to eliminate administrative burden, delivering measurable ROI — up to 6 hours saved per team per day.

**Website:** [cura-co.com](https://cura-co.com)  
**Contact:** dan@cura-co.com
