# DataIsCool — Brand Guide v2.0

## Brand Essence

**One sentence:** Standing on a rock overlooking a misty forest valley — adventurous, natural, warm, and quietly confident.

**Three words:** Adventurous · Natural · Warm

**Personality:** Like a cozy cabin in the woods. Not tech-heavy. Not clinical. Personal, human, grounded in nature.

**Tone of voice:** Friendly but not childish · calm, never urgent · feels handmade and personal · like a recipe written in a journal

---

## Colour Palette

Extracted directly from the brand image. The palette has four families:

### 1. Cream / Ivory — the page
Warm background and primary text tones. The "paper" the brand is written on.

| Token        | Hex       | Use |
|---|---|---|
| `cream-bg`   | `#f0ebe0` | Page background (hub, light areas) |
| `cream-white`| `#f5f0e8` | Primary text, headings on dark |
| `cream-light`| `#e8e0d0` | Body text on dark backgrounds |
| `cream-muted`| `#c8bca8` | Secondary text, labels |
| `cream-dim`  | `#9a8e7c` | Placeholder, disabled |
| `cream-faint`| `#6a5e4e` | Very subtle captions |

### 2. Forest Green — the nature backbone
Backgrounds, surfaces, depth. Multiple layers like the mountain ranges in the image.

| Token        | Hex       | Use |
|---|---|---|
| `forest-deep`| `#1a2e20` | Deepest background |
| `forest-dark`| `#1f3626` | App background |
| `forest-mid` | `#2a4232` | Cards, panels |
| `forest-light`| `#334e3e` | Elevated cards, hover |
| `forest-mist`| `#3d5c4a` | Borders, dividers |
| `forest-edge`| `#4a6858` | Subtle borders |

### 3. Navy — the logo and text authority
From the glasses frame and the "DataIsCool" wordmark. Grounds the brand.

| Token        | Hex       | Use |
|---|---|---|
| `navy-deep`  | `#1a2440` | Logo frame, dark text on light |
| `navy-mid`   | `#2a3860` | Headings on cream backgrounds |
| `navy-soft`  | `#4a5878` | Secondary text on cream |

### 4. Teal / Sage — the accent
From the bar charts inside the glasses lens. The interactive, alive colour.

| Token        | Hex       | Use |
|---|---|---|
| `teal`       | `#3a9a8a` | Primary buttons on cream bg |
| `sage`       | `#6db870` | Primary buttons on dark bg, active nav |
| `sage-light` | `#8dd090` | Hover state |
| `sage-glow`  | `rgba(109,184,112,0.15)` | Selected card bg |

### 5. Amber / Gold — the warmth accent
From the trend line in the glasses. Used sparingly.

| Token   | Hex       | Use |
|---|---|---|
| `amber` | `#c8a84b` | Star ratings, gold highlights |

### Semantic

| Token     | Hex       |
|---|---|
| `danger`  | `#c0524a` |
| `success` | `#5cb85c` |

---

## Typography

| Role    | Font              | Use |
|---|---|---|
| Display | DM Serif Display  | Page titles, recipe names, section headings — always cream white on dark |
| UI      | Syne              | Navigation, buttons, body text — the workhorse |
| Mono    | DM Mono           | Metadata, tags, timestamps, UPPERCASE labels ONLY |

### Hierarchy (dark backgrounds)
1. **Page title** — DM Serif Display 32–48px, `cream-white #f5f0e8`
2. **Section heading** — DM Serif Display 20–28px, `cream-white #f5f0e8`
3. **Card title** — DM Serif Display 17–20px, `cream-white #f5f0e8`
4. **Body** — Syne 14–16px, `cream-light #e8e0d0`
5. **Label** — DM Mono 10–11px UPPERCASE, `cream-muted #c8bca8`
6. **Caption** — Syne 12–13px, `cream-dim #9a8e7c`

### Rules
- **Never** green text on green background
- **Never** pure white `#ffffff` — always cream
- **Never** pure black — use navy-deep or forest-deep
- DM Mono is for labels/metadata ONLY — never body text

---

## Surfaces (dark theme — recipe app)

| Level  | Background | Border | Use |
|---|---|---|---|
| Base   | `rgba(26,46,32,0.85)` + blur(16px) | `rgba(245,240,232,0.08)` | Cards, panels |
| Raised | `rgba(20,38,28,0.95)` + blur(20px) | `rgba(245,240,232,0.10)` | Sticky headers, modals |
| Sunken | `rgba(14,28,20,0.75)` | `rgba(245,240,232,0.06)` | Inputs, text areas |

---

## Background System

The brand background always has three layers:

1. **Sky** — cream/ivory at the very top, fading into mist green
2. **Mountains** — multiple SVG silhouette layers, each slightly darker
3. **Ground** — dark forest fade at the bottom where content lives

This is the visual signature of DataIsCool. Never just a flat colour.

---

## Logo

The DataIsCool logo consists of:
- **Glasses frame** — navy-deep `#1a2440`, thick rounded stroke
- **Left lens** — bar chart in teal blues (from brand image: blues/teals)
- **Right lens** — trend line with dots in teal/blue
- **Wordmark** — "DataIsCool" in navy-deep, the "I" highlighted in teal

In app contexts (small, on dark bg):
- Frame stroke: cream-white `#f5f0e8`
- Bar chart: sage `#6db870`
- Trend line: amber `#c8a84b`

---

## Components

### Buttons
- **Primary (dark bg):** sage `#6db870` · forest-deep text · Syne Bold 15px · 12px radius · 44px min height
- **Primary (light bg):** teal `#3a9a8a` · cream-white text
- **Secondary:** glass surface · cream-muted border/text
- **Danger:** `#c0524a` · cream-white text

### Cards
- Glass Base surface (dark bg) or cream-bg with navy border (light bg)
- DM Serif Display title in cream-white
- DM Mono category label in cream-muted
- Hover: translateY(-3px) + `0 8px 32px rgba(0,0,0,0.4)`
- Selected: sage-glow bg + sage border

### Navigation
- **Mobile:** Fixed bottom · glass raised · sage active · DM Mono 9px labels
- **Desktop:** Top tab bar · sage underline · DM Mono 11px labels

### Inputs
- Sunken surface
- cream-light text, cream-dim placeholder
- Sage border on focus
- DM Mono UPPERCASE label above

### Past vs Future (Planner)
- **Past days:** opacity 0.4, no interactive elements
- **Today:** sage-glow background + sage border + "TODAY" label in sage
- **Future:** normal glass surface
- These must be visually distinct — never subtle

---

## Spacing Scale

| xs | sm | md | lg | xl | 2xl |
|---|---|---|---|---|---|
| 4px | 8px | 16px | 24px | 40px | 64px |

---

## Do / Don't

**Do:**
- Cream text on forest backgrounds — always
- Layer the forest background — it's the signature
- DM Serif Display for anything the user reads (titles, names)
- Make past days obviously inactive (opacity + no buttons)
- Use navy on cream surfaces, cream on forest surfaces

**Don't:**
- Green text on green — ever
- Pure white or pure black
- DM Mono for body text
- Flat colour backgrounds — always the forest
- Same visual weight for everything — establish clear hierarchy

