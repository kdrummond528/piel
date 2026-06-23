# Piel — pieltattoo.com

Family-made temporary tattoo brand. Two sisters, one daughter, she draws everything.

## What this repo is

Static website for **pieltattoo.com**, hosted on GitHub Pages. No build step, no framework — just HTML and CSS.

---

## File structure

```
/
├── index.html       # Main site (one-page layout)
├── style.css        # All styles
├── logo.png         # Piel Habla logo
└── README.md        # This file
```

---

## Sections on the site

1. **Hero** — Logo + tagline "ni de aquí ni de allá"
2. **About** — Brand story, three product lines (Libre, Habla, Edición)
3. **Coming Soon** — West Seattle launch collection (Troll, Whale Tail, Ferry)
4. **Contact** — Wholesale + Piel Habla partnership emails

---

## Brand tokens

| Token | Value | Use |
|-------|-------|-----|
| `--gold` | `#F2A81D` | Accents, badges, highlights |
| `--terra` | `#B85042` | Buttons, brand line labels |
| `--sage` | `#7A9E8E` | Eyebrows, subtle text |
| `--cream` | `#FAF6EF` | Page background |
| `--dark` | `#1E1410` | Coming soon section bg, footer |
| `--mid` | `#6B5B4E` | Body text |
| `--light-sage` | `#D6E8E1` | Contact section bg |

Fonts: **Fraunces** (display/headings, serif) + **DM Sans** (body) — loaded from Google Fonts in `index.html`.

---

## To make edits

Open the repo folder in VS Code, edit `index.html` or `style.css`, then:

```bash
git add -A
git commit -m "describe what you changed"
git push
```

GitHub Pages rebuilds automatically. Changes go live in ~30 seconds.

---

## DNS (Porkbun → GitHub Pages)

Domain: `pieltattoo.com` registered on Porkbun.

DNS A records pointing to GitHub Pages IPs:
```
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```

CNAME: `www` → `kdrummond528.github.io`

HTTPS enforced via GitHub Pages settings.

---

## What's still to do

- [ ] Add real design images to the three Coming Soon cards (Troll, Whale Tail, Ferry)
- [ ] Confirm contact emails (`hello@pieltattoo.com`, `habla@pieltattoo.com`) are set up
- [ ] Add social links (Instagram, TikTok) to footer once handles are live
- [ ] Piel Habla AAC line detail page (Phase 2)
- [ ] Wholesale one-pager as downloadable PDF
- [ ] Launch Piel Edición seasonal drop section when ready

---

## Product lines

| Line | Description | Channel | Price |
|------|-------------|---------|-------|
| Piel Libre | Core sketchbook collection, quarterly rotations | Boutiques, bookstores, gift | $3 WS / $8–10 RT |
| Piel Habla | AAC line — Dime, Siento, Juntos sets | Therapy supply, hospitals, D2C | $10–18 RT |
| Piel Edición | Seasonal cultural drops | All channels | $4.50 WS / $9–12 RT |
| Piel x [Name] | Guest collabs with Hispanic illustrators | Community/PR | Variable |

## Launch collection — West Seattle

| Code | Name | Location | Detail |
|------|------|----------|--------|
| TT | The Troll | Bruun Idun · Lincoln Park | Hidden bird in his hair |
| WT | Whale Tail | La Cola · Alki Beach | Ghosted Seattle skyline |
| TF | The Ferry | El Ferry · Fauntleroy | Hidden family in one window |