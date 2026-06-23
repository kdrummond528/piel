# CLAUDE.md — Piel / pieltattoo.com

This file is for Claude Code. Read it before touching anything.

---

## What we're building

Static website for **pieltattoo.com** — a family-made temporary tattoo brand called Piel. No framework, no build step. Just HTML, CSS, and a logo image. Hosted on GitHub Pages.

The brand has two lines with separate domains:
- `pieltattoo.com` — main brand (this repo)
- `pielhabla.com` — accessibility/AAC line (future, same owner)

---

## Stack

- Plain HTML + CSS (no React, no bundler, no npm)
- GitHub Pages (auto-deploys on push to main)
- Google Fonts: Fraunces (headings) + DM Sans (body)
- No backend, no CMS, no JS framework

To deploy: `git add -A && git commit -m "message" && git push`

---

## File structure

```
/
├── index.html       # One-page site, all sections
├── style.css        # All styles, CSS variables at top
├── logo.png         # Piel Habla logo (do not move or rename)
├── CLAUDE.md        # This file
└── README.md        # Human-facing docs
```

---

## Brand tokens (CSS variables in style.css)

```css
--gold: #F2A81D        /* accents, badges */
--terra: #B85042       /* buttons, brand labels */
--sage: #7A9E8E        /* eyebrows, subtle text */
--cream: #FAF6EF       /* page background */
--dark: #1E1410        /* coming soon bg, footer */
--mid: #6B5B4E         /* body text */
--light-sage: #D6E8E1  /* contact section bg */
```

Fonts: Fraunces (serif, display) + DM Sans (sans, body). Both loaded via Google Fonts link in `<head>`.

---

## Site sections (in order)

1. **Nav** — fixed top, links to About / Coming Soon / Contact
2. **Hero** — logo (floating animation) + tagline "ni de aquí ni de allá"
3. **About** — brand story + three product lines as a ruled list
4. **Coming Soon** — three West Seattle launch designs as cards
5. **Contact** — two cards (wholesale + Piel Habla), email buttons
6. **Footer** — copyright + tagline

---

## Brand context

- Two sisters co-founding. 12-year-old niece draws every design — that's the moat.
- Florida born, Hispanic, living between cultures. "Ni de aquí ni de allá."
- Every design has a hidden detail — call this out in copy wherever relevant.
- Voice: warm, specific, bilingual-friendly. Not precious. Not corporate.

### Product lines

| Line | Concept | Channel |
|------|---------|---------|
| Piel Libre | Core sketchbook collection, quarterly drops | Boutiques, bookstores, gift shops |
| Piel Habla | AAC tattoos for nonverbal kids, Deaf families | Therapy supply, hospitals, D2C |
| Piel Edición | Seasonal cultural drops (Día de los Muertos, etc.) | All channels |
| Piel x [Name] | Collabs with Hispanic illustrators | Community/PR |

### West Seattle launch collection

| Code | Name | Hidden detail |
|------|------|---------------|
| TT | The Troll (Bruun Idun · Lincoln Park) | Hidden bird in his hair |
| WT | Whale Tail (La Cola · Alki Beach) | Ghosted Seattle skyline |
| TF | The Ferry (El Ferry · Fauntleroy) | Hidden family in one window |

---

## To-do list (pick up here)

- [ ] Add real design images to the three Coming Soon cards
- [ ] Confirm and update contact emails (currently placeholder: hello@ and habla@pieltattoo.com)
- [ ] Add social links to footer (Instagram, TikTok) once handles are confirmed
- [ ] Add a `CNAME` file if it gets wiped (contents: `pieltattoo.com`)
- [ ] Piel Habla detail section or separate page (Phase 2)
- [ ] Wholesale one-pager as downloadable PDF
- [ ] Piel Edición seasonal drop section

---

## DNS / hosting notes

- Domain on Porkbun, DNS pointed to GitHub Pages IPs
- Custom domain set in GitHub Pages settings
- HTTPS enforced
- CNAME file in repo root (contents: `pieltattoo.com`) — don't delete it

---

## Rules for this repo

- Keep it static. No build tools, no node_modules, no frameworks unless explicitly discussed.
- All styles in `style.css`. No inline styles.
- Mobile-first. Test at 375px and 1280px.
- Don't change font families without asking — Fraunces + DM Sans is intentional.
- Don't change the CSS variable names — they're used throughout.