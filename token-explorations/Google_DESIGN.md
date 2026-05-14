---
name: Cara
colors:
  primary: "#FF5D00"
  primary-subtle: "rgba(255, 93, 0, 0.1)"
  black: "#000000"
  white: "#FFFFFF"
  gray-light: "#F9F9F9"
  gray-mid: "#EDEDED"
  gray-text: "#6B6B6B"
typography:
  display:
    fontFamily: Manrope
    fontSize: 3.75rem
    fontWeight: 500
    lineHeight: 1.25
    letterSpacing: 0.05em
  subheading:
    fontFamily: Manrope
    fontSize: 1.625rem
    fontWeight: 500
    lineHeight: 1.5
    letterSpacing: 0.05em
  label:
    fontFamily: Manrope
    fontSize: 1.125rem
    fontWeight: 700
    lineHeight: 1
    letterSpacing: 0.05em
  caption:
    fontFamily: Manrope
    fontSize: 0.875rem
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: 0.05em
  wordmark:
    fontFamily: BBH Hegarty
    fontSize: 2.75rem
    fontWeight: 400
rounded:
  button: 40px
  card: 20px
  nav: 30px
spacing:
  section-vertical: 100px
  section-horizontal: 150px
  column-gap: 80px
  element-gap: 20px
  element-gap-lg: 40px
---

## Overview

Cara is an electric bicycle brand on a mission to provide car-alternatives for a better world. The tagline: *"Electric bicycles for everyday life. Racks are the new trunk."* The brand is elevated, friendly, active, fresh, soft, and joyful — rooted in everyday urban mobility. The product is the Cara C1, a Class 2 e-bike with a 40-mile range at $1,399, designed for daily commuting and errands.

Every design decision should reinforce that riding Cara feels optimistic, effortless, and unmistakably modern — not sporty or techy, but warmly human.

## Colors

The palette is built around a single bold accent against clean neutrals, giving Cara an energetic but uncluttered presence.

- **Primary (#FF5D00):** Cara orange — the brand's defining color. Used for CTA buttons, links, accent text, the logo, and any interactive element. It should never be overused; it earns its energy through restraint.
- **Primary-subtle (rgba(255,93,0,0.1)):** A barely-there orange tint for section backgrounds and hover states where warmth is needed without intensity.
- **Black (#000000):** Body text, spec labels, and any high-contrast readable content.
- **White (#FFFFFF):** Reversed text on dark or photographic backgrounds, and button labels on orange fills.
- **Gray-light (#F9F9F9):** Footer background and soft section surfaces — slightly off-white for warmth.
- **Gray-mid (#EDEDED):** Product section background — neutral enough to let the peach/cream bicycle pop without competing.
- **Gray-text (#6B6B6B):** Subtext, captions, footer taglines, and secondary labels. Never used for primary reading content.

## Typography

Two typefaces only. Their roles are strict and should never be swapped.

- **BBH Hegarty Regular** is reserved exclusively for the "cara" wordmark in the header and footer. It is the brand's signature — do not use it for any other copy.
- **Manrope Variable** handles everything else. It is the workhorse of the UI: clean, geometric, and airy. The consistent 0.05em letter-spacing across all sizes gives the brand its open, unhurried feel.

Headlines use sentence case with a terminal period — a distinctive stylistic choice that gives finality and weight. Navigation and button labels use Title Case. Body copy and captions use sentence case without a period unless a full sentence.

## Spacing

Spacing is generous. White space is not wasted — it is the design. Sections breathe with 100px vertical padding and 150px or more of horizontal margin at 1440px. This generosity signals a premium, considered product without the rigidity of a luxury brand.

Do not compress spacing to fit more content. Prioritize hierarchy and breathing room over density.

## Components

### Buttons

Two button variants, both fully pill-shaped (border-radius: 40px). No shadows. Flat and direct.

- **Primary:** Orange fill (#FF5D00), white Manrope Bold 18px text, 0.05em tracking. Used for the main CTA — "Sign Up", "Explore".
- **Outline:** Orange border and orange text, transparent fill. Used for secondary actions — "Learn More". Same sizing and type as primary.

Hover states: reduce opacity to ~0.8 or slightly darken the fill. No scale transforms. No shadows added on hover.

### Navigation

A floating pill-shaped header with 30px border radius. Frosted glass treatment: layered `rgba(255,255,255,0.25)` and `rgba(0,0,0,0.2)` backgrounds. Nav items are Manrope Bold 18px in Title Case. The primary CTA ("Sign Up") sits as an orange pill button in the header. The "cara" wordmark in BBH Hegarty anchors the left side.

### Cards

Cards and image frames use 20px border radius — soft, not sharp. No drop shadows. Depth is achieved through background color changes and photography, not elevation.

## Imagery

Warm, natural, and earthy. Lifestyle photography features real people riding, carrying groceries, and navigating urban scenes. Product photography sits on clean neutral backgrounds. All photography carries a warm, slightly muted colour grade — not over-saturated, not dramatic. Circle crops are used selectively for community or fleet imagery.

No illustrations. No hand-drawn elements. No icons in the navigation or footer — these areas are text-only. If iconography is needed (e.g. feature lists), use Lucide icons at 2px stroke weight — clean and geometric, matching the brand's open aesthetic.

## Voice & Tone

Conversational and optimistic. Headlines are short, punchy, and declarative with real rhythm: *"A new way to move."*, *"Better in bunches."*, *"Racks are the new trunk."* The brand never sounds corporate. It speaks directly to the rider through implied second-person benefit statements. No emoji. No exclamation marks used for enthusiasm — the words carry the energy on their own.
