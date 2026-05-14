# Cara — Design System

## Brand & Purpose

Cara is an electric bicycle brand positioned as a car-alternative for everyday urban life. The visual language is warm, confident, and approachable — blending the clean modernism of premium mobility brands with an earthy, sustainable palette. The aesthetic avoids "techy" coldness in favour of accessibility and optimism.

---

## Color Palette

| Token         | Hex       | Usage                                              |
|---------------|-----------|----------------------------------------------------|
| `--orange`    | `#E84B0F` | Primary brand color. CTAs, logos, accents, icons   |
| `--cream`     | `#FFF5EE` | Page background, hero text sections                |
| `--peach`     | `#F9E8D8` | Feature icon backgrounds, fleet section fill       |
| `--dark`      | `#111111` | Primary text, headings                             |
| `--mid`       | `#555555` | Secondary text, specs, captions, nav links         |
| `--light-gray`| `#F2F0EE` | Alternate section background (product section)     |
| `--bike-peach`| `#F5C9A0` | Decorative radial gradient behind product image    |

**Hover / Active States:**
- Orange hover: `#C43E0B` (darkened ~15%)
- Orange shadow glow: `rgba(232,75,15,0.35)` on buttons

---

## Typography

### Typefaces

| Family        | Role                         | Source            |
|---------------|------------------------------|-------------------|
| **BBH Hegarty** | Brand logotype, wordmark   | Google Fonts      |
| **Manrope**   | All UI text and headings     | Google Fonts      |

### Type Scale

| Element              | Size    | Weight | Letter Spacing | Notes                        |
|----------------------|---------|--------|----------------|------------------------------|
| Logo / Wordmark      | 34px    | 400    | -0.5px         | BBH Hegarty, orange          |
| Section H2           | 60px    | 500    | -1px           | Manrope; scales to 36–40px mobile |
| Hero H1              | 60px    | 500    | -1px           | Manrope; scales to 36px mobile |
| Fleet H2             | 60px    | 500    | -1px           | Manrope, orange color        |
| Feature Card H3      | 17px    | 700    | -0.2px         | Manrope                      |
| Body / Paragraph     | 15–17px | 400    | —              | Line-height 1.5–1.65         |
| Product Specs        | 15px    | 500    | —              | `--mid` color, line-height 1.8|
| Product Price        | 28px    | 700    | —              | `--dark` color               |
| Product Tag / Label  | 11px    | 700    | 0.15em         | Uppercase, orange            |
| Nav Links            | 14px    | 500    | 0.02em         | White on hero; dark on scroll|
| Footer Column Heads  | 12px    | 700    | 0.1em          | Uppercase, `--mid`           |
| Footer Links         | 14px    | 400    | —              | `--dark`; orange on hover    |
| Footer Brand Tagline | 12px    | 400    | —              | `--mid`                      |
| Button               | 14px    | 600    | —              | Manrope                      |

---

## Spacing & Layout

### Grid

- Desktop base: `60px` horizontal padding on all major sections
- Mobile: `24px` horizontal padding
- Section min-height: `85vh` (hero: `90vh` mobile)
- Product section: `2-column` CSS grid (`1fr 1fr`), collapses to single column on mobile
- Fleet section: `2-column` CSS grid (`1fr 1fr`), collapses to single column on mobile
- Features grid: `3-column` CSS grid with `40px` gap; collapses to `1-column` on mobile
- Footer: `grid-template-columns: 200px 1fr`; collapses to `1-column` on mobile

### Section Padding

| Section   | Desktop Padding         | Mobile Padding        |
|-----------|-------------------------|-----------------------|
| Nav       | 20px 60px               | 16px 24px             |
| Hero      | padding-bottom: 80px    | padding-bottom: 56px  |
| Product   | 80px 60px (left panel)  | 56px 24px / 36px 24px |
| Features  | 80px 60px               | 56px 24px             |
| Fleet     | 80px 60px (left panel)  | 56px 24px             |
| Footer    | 60px                    | 48px 24px 40px        |

---

## Components

### Navigation

- Fixed, full-width, transparent by default
- On scroll (`scrollY > 60`): transitions to `rgba(255,245,238,0.40)` with `backdrop-filter: blur(20px)` and a subtle orange-tinted bottom border (`rgba(232,75,15,0.08)`)
- Logo: BBH Hegarty, 34px, orange
- Links: Manrope 14px/500, white on hero; switch to `--dark` on scroll
- CTA pill ("Sign Up"): orange background, white text, `border-radius: 100px`, 10px 22px padding
- Mobile: hamburger menu (3-bar icon → X animation), nav links expand into a dark blurred overlay panel (`rgba(17,17,17,0.96)`)

### Buttons

Three variants, all `border-radius: 100px` (pill shape), Manrope 14px/600:

| Variant          | Background   | Text    | Border              | Hover                                      |
|------------------|--------------|---------|---------------------|--------------------------------------------|
| `.btn-orange`    | `#E84B0F`    | white   | none                | `#C43E0B` bg + `translateY(-2px)` + glow  |
| `.btn-outline`   | transparent  | orange  | 1.5px solid orange  | Fills orange, white text + `translateY(-2px)` + glow |
| `.btn-outline-dark` | transparent | white | 1.5px solid `rgba(255,255,255,0.6)` | Fills white, dark text + lift |

Base padding: `12px 28px`. Nav CTA: `10px 22px`.

### Feature Cards

- Background: white
- Border: `1px solid rgba(0,0,0,0.06)`
- Border-radius: `16px`
- Padding: `36px` (mobile: `28px 24px`)
- Hover: `translateY(-6px)` + `box-shadow: 0 16px 40px rgba(0,0,0,0.08)`
- Icon container: `40×40px`, `--peach` background, `border-radius: 10px`, orange stroke icon (20px SVG)
- Transition: `0.25s` on transform and shadow

### Hero Section

- Full-bleed video background (`object-fit: cover`)
- Overlay gradient: `linear-gradient(to top, rgba(0,0,0,0.65) 0%, rgba(0,0,0,0.2) 50%, rgba(0,0,0,0.1) 100%)`
- Content anchored to bottom-left (`justify-content: flex-end`, `padding-bottom: 80px`)
- Max-width: `900px` for hero text block

### Product Section

- Left: light-gray background (`--light-gray`), text content with tag, heading, specs, price, CTA
- Right: white background with `radial-gradient` peach glow (500×500px circle at center)
- Bike image: `drop-shadow(0 30px 50px rgba(0,0,0,0.12))`, hover: `scale(1.03) translateY(-6px)` over `0.6s`

### Fleet Section

- Background: `--peach`
- Heading rendered in `--orange`
- Dashboard image: `border-radius: 16px`, `box-shadow: 0 30px 80px rgba(0,0,0,0.15)`, hover: `scale(1.02) rotate(-1deg)` over `0.4s`

### Footer

- Background: `#F9F9F9` (near-white, slightly off cream)
- Two-column grid: brand on left, 4-column link grid on right
- Column headers: 12px, 700, uppercase, `--mid`

---

## Motion & Animation

### Scroll Reveal

All major content blocks use an `.reveal` class with IntersectionObserver (threshold: `0.12`):

- Initial state: `opacity: 0; transform: translateY(28px)`
- Active state: `opacity: 1; transform: translateY(0)`
- Duration: `0.7s ease`
- Staggered delays: `.reveal-delay-1` (0.1s), `.reveal-delay-2` (0.2s), `.reveal-delay-3` (0.3s)

### Other Transitions

| Element              | Property          | Duration  | Easing     |
|----------------------|-------------------|-----------|------------|
| Nav background       | background        | 0.4s      | ease       |
| Nav link color       | color             | 0.2s      | —          |
| Buttons (all)        | transform, shadow | 0.18s     | —          |
| Feature cards        | transform, shadow | 0.25s     | —          |
| Bike image hover     | transform         | 0.6s      | ease       |
| Dashboard hover      | transform         | 0.4s      | ease       |
| Hamburger bars       | transform, opacity| 0.3s      | ease       |
| Nav mobile panel     | max-height, opacity| 0.4s/0.3s| ease       |

---

## Responsive Breakpoint

**Single breakpoint: `max-width: 768px`**

Key mobile changes:
- Nav collapses to hamburger + expandable dark overlay menu
- All multi-column grids (`product`, `fleet`, `features`) collapse to single column
- In product section, image panel (`product-right`) renders above text (`order: 1 / order: 2`)
- Section heading sizes reduce from 60px → 36–40px
- Horizontal padding reduces from 60px → 24px
- Footer link columns collapse from 4-column grid to 2-column grid
- Buttons go full-width inside flex containers

---

## Design Principles

1. **Warmth over tech** — Cream and peach tones, earthy orange, approachable typography. Deliberately avoids cold blues, hard blacks, or hyper-minimalist aesthetics.
2. **Motion as delight** — Hover lifts, subtle rotations, and staggered reveals reward attention without feeling gratuitous.
3. **Orange as conviction** — The single brand color does all the heavy lifting: logo, CTAs, icons, accent text, and hover states. Nothing competes with it.
4. **Large, confident headings** — 60px at weight 500 with tight tracking (-1px) creates editorial authority without aggression.
5. **Photography-first** — Full-bleed video hero and product imagery carry the emotional weight; UI steps aside to support them.
