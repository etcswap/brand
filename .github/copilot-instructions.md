# ETCswap Brand Repository — Copilot Instructions

## Project

Brand assets repository for ETCswap (decentralized exchange on Ethereum Classic). Contains logos, favicons, social cards, design tokens, and brand guidelines.

## Key Rules

- Primary brand color: `#33FF99`
- Dark backgrounds: `#131313` (standard), `#030508` (deep)
- Font: DM Sans (Google Fonts), weights 400-700
- Logomark is a 3-path geometric SVG — never modify the path data
- All PNGs are generated from SVGs using ImageMagick
- SVG files are the source of truth

## Protected Files

- `logo/logomark-green.svg` — canonical brand mark, do not alter paths
- `README.md` — brand guidelines, update carefully

## Asset Generation

```bash
convert -background none logo/logomark-green.svg -resize [SIZE]x[SIZE] output.png
```
