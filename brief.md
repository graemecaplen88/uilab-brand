# UiLab — brand brief

*Paste this into Lovable's Knowledge panel (or any AI builder / Claude project) so
generations stay on-brand. UiLab is an **innovation lab in Logan, South East Queensland**
— "translating emerging technology into local success." Place-based, practical, optimistic.*

---

## ⭐ Headline prompt (drop-in for any agent / AI tool)

> Copy the block below verbatim into a system prompt, Cursor/Claude rules file, or chat.
> It assumes the agent can read the GitHub repo `graemecaplen88/uilab-brand`.

```text
You are designing for UiLab — an innovation lab in Logan, South East Queensland whose
mission is "translating emerging technology into local success." Voice: plain, declarative,
local, optimistic; sentence case for everything readable, ALL-CAPS Roboto Mono for labels/
eyebrows/names/URLs, underline key words for emphasis. No emoji, no hype. Australian English.

Apply the brand with ONE hard rule: the background is always the DARKER tone and the text/
logo/graphics are always the LIGHTER tone. Build each surface from one dark ground +
one light "pop" accent (one primary action per view):
  Dark grounds — Sunset #4C0027 · Water/navy #013053 · Earth #421C01 · Land/forest #025120
  Light pops   — Summer #FF6325 · Sky #67DAFF · Sun #FFCD0E · Jacaranda #DD60FF
  Flagship pairing = Water ground + Sun pop (navy + yellow).
Type: PP Neue Montreal for display/body (sentence case, tight tracking); Roboto Mono Bold
uppercase for labels. Tight radii (2–10px, square-tittle DNA), hairline white-alpha borders,
depth from layered tone not heavy shadow, 4pt spacing, crisp 120–280ms ease-out motion,
2px accent focus ring. Recurring motif: the Logan council "Divisions" silhouettes as faint
backgrounds / masks / solid pop-coloured shapes. Tagline: "Translating emerging technology into local success." Verticals:
Community · Connect · Events · Podcasts · Industry. Icons: brandmark + mono letter-marks +
colour status pips; thin outline (Lucide) only for functional glyphs — never emoji.

Find the source files in the repo github.com/graemecaplen88/uilab-brand:
  • Brand marks/  and  Word marks/      → logo SVG/PNG in 10 themes (use the *.svg)
  • 5. Logan Divisions Graphics/         → the Logan map / division silhouettes
  • 6. Font Files/                        → PP Neue Montreal .otf + Roboto Mono
  • 7. Platform icons, backgrounds…/      → banners, virtual backgrounds, social
  • UiLab Brand Guidelines …August 2025.pdf  → full guidelines (colour/type/logo/grid)
If a UiLab "design system" project is connected, also read: styles.css (token entry),
tokens/*.css (colours, type, spacing, effects), components/* (Button, Card, Tag, Input,
Select, Switch, Tabs, Avatar, StatusDot) and ui_kits/website/ (a full site recreation).
Always read the real assets/tokens before designing; never invent off-brand colours or type.
```

---

## Voice & copy
- **Plain, declarative, local.** Short confident statements. Lead with the point.
  "A place for Logan to grow and succeed." "Translating emerging technology into local success."
- Address the reader as **"you."** The product/org is **"UiLab."**
- **Sentence case** for everything readable (headings, body, card titles).
  **ALL-CAPS mono** for eyebrows, names, roles, URLs, tags, metadata
  (`STEFAN MARTIN`, `FULL STACK DEVELOPER`, `UILAB.COM.AU`, `EMERGING TECH / 2025`).
- **Underline key words** for emphasis (skip-ink), never bold or colour-shift:
  "Translating <u>emerging technology</u> into <u>local success</u>."
- **No emoji. No hype** ("unlock / supercharge / seamless / revolutionary" are banned).
- **Australian English** (organise, colour, neighbourhood). Name real places & people
  (Logan, Brisbane, South East Queensland, council divisions).
- Tone words: grounded · precise · community · emerging · practical · welcoming.

## The one colour rule (non-negotiable)
**The background is ALWAYS the darker tone; text / logo / graphics are ALWAYS the lighter
tone.** Each surface = one **dark ground** + one **light pop** (the pop is the single vivid
accent — one primary action per view). Never put a dark mark on a light brand colour.

### Palette
| Role | Name | Hex |
|---|---|---|
| Dark ground | Sunset | `#4C0027` |
| Dark ground | Water (navy) | `#013053` |
| Dark ground | Earth | `#421C01` |
| Dark ground | Land (forest) | `#025120` |
| Light pop | Summer (orange) | `#FF6325` |
| Light pop | Sky (blue) | `#67DAFF` |
| Light pop | Sun (yellow) | `#FFCD0E` |
| Light pop | Jacaranda (violet) | `#DD60FF` |
| Neutral | Black / White / Paper | `#000000` / `#FFFFFF` / `#F4F1EC` |

**Canonical pairings:** Water + Sun (flagship navy/yellow) · Sunset + Summer · Land + Sky ·
Earth + Sun. Depth = layered surface tones + hairline borders (white at low alpha), not
heavy shadow. The only "glow" is a faint accent radial behind a hero element.

## Type
- **Display & body: PP Neue Montreal** (licensed; nearest free swap = Hanken Grotesk).
  Sentence case, tight tracking on large sizes. Weights: Light/Regular/Medium/SemiBold/Bold.
- **Labels & data: Roboto Mono** — **Bold, UPPERCASE, wide tracking (~0.14em)** for
  eyebrows, tags, names, URLs, table headers, figures.
- Signature move = a big confident grotesque headline over a small precise mono kicker.

## Shape, spacing, motion
- **Tight radii** (2–10px). The wordmark "i" has a **square tittle** — keep corners
  architectural. Pills only for status dots & avatars.
- **4pt spacing scale.** Layout on a **6-column grid** (square/web, extends to 12) or
  **4-column** (vertical/editorial). Generous margins; white space is part of the system.
- **Motion:** crisp, 120–280ms ease-out. Fades + small (2–4px) translations; buttons
  scale to 0.975 on press. No bounce, no decorative loops.
- **States:** hover lightens one step; press darkens + scales down; focus = **2px accent
  ring**, offset.

## Logo & motif
- **Wordmark** "UiLab" (geometric + humanist, square i-tittle). **Brandmark** = a columned
  people/colonnade form, "two halves meeting in the middle" — a bridge between people &
  systems. Both ship in every theme colour.
- **Graphic motif: the Logan "Divisions"** — silhouettes of Logan's 12 council boundaries,
  used as faint background motifs, framing devices, solid pop-coloured shapes, or image
  masks. Tagline that pairs with them: **"Translating emerging technology into local success"**
- **Verticals:** Community · Connect · Events · Podcasts · Industry (lock up to the
  wordmark in Title Case).

## Icons
No bespoke icon set. Use the brandmark, **mono letter-marks** (initials/avatars) and
**colour status pips** (never emoji). For functional glyphs (chevrons, arrows, close) use a
thin **outline** set such as **Lucide** (1.5–2px stroke). Avoid filled/duotone/playful icons.

---

## Tailwind / shadcn quick config
For Lovable-style stacks (dark-first; set `<html class="dark">`).

```js
// tailwind.config — theme.extend
colors: {
  sunset: '#4C0027', water: '#013053', earth: '#421C01', land: '#025120',
  summer: '#FF6325', sky: '#67DAFF', sun: '#FFCD0E', jacaranda: '#DD60FF',
  paper:  '#F4F1EC',
  // semantic (flagship Water + Sun)
  background: '#013053',
  foreground: '#FFFFFF',
  primary: '#FFCD0E',            // the pop; dark text on it
  'primary-foreground': '#013053',
  border: 'rgba(255,255,255,0.16)',
},
fontFamily: {
  sans: ['PP Neue Montreal', 'Hanken Grotesk', 'system-ui', 'sans-serif'],
  mono: ['Roboto Mono', 'ui-monospace', 'monospace'],
},
letterSpacing: { tight: '-0.03em', label: '0.14em' },
borderRadius: { lg: '10px', md: '6px', sm: '4px' },
```

```css
/* eyebrow / label helper */
.eyebrow { font-family: 'Roboto Mono'; font-weight: 700; text-transform: uppercase;
           letter-spacing: 0.14em; color: var(--primary); font-size: 0.8125rem; }
```

**Prompt pattern:** *"Following the UiLab brief — dark Water ground, Sun-yellow primary,
PP Neue Montreal headlines in sentence case with Roboto Mono uppercase eyebrows, tight
radii, hairline borders, a faint Logan-divisions silhouette behind the hero. One primary
action. No emoji, no hype."*

---

## Source repo
Full brand assets (logos & wordmarks in 10 themes, Logan division graphics, fonts,
guidelines PDF, social templates): **https://github.com/graemecaplen88/uilab-brand** —
explore it for higher-fidelity artwork than any single export.

*Translating emerging technology into local success.*
