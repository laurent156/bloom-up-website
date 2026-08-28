---
name: Bloom Up
description: Collagen café & beauty bar in Mons, Grands Prés — franchise-scale brand system, warm and editorial
colors:
  terracotta-bold: "#B45F52"
  wisteria-bloom: "#7047D7"
  espresso-brown: "#4A352D"
  soft-nude: "#D8B8AE"
  rose-clay: "#C88F86"
  warm-cream: "#F5EFEA"
  charcoal-brown: "#1F1A18"
  warm-coral: "#C96E5E"
  hairline: "#E4D5CC"
  signal-red: "#A90318"
  bright-lavender: "#9A70E8"
  berry-pink: "#D64F8C"
  ultramarine: "#4D5AC7"
  sunny-yellow: "#F2C84B"
  acid-lime: "#B8D34B"
typography:
  display:
    fontFamily: "Skinova, Georgia, serif"
    fontSize: "clamp(60px, 6.5vw, 104px)"
    fontWeight: 400
    lineHeight: 0.97
    letterSpacing: "0.01em"
  headline:
    fontFamily: "Playfair, PlayfairDisplay, Georgia, serif"
    fontSize: "48px"
    fontWeight: 500
    letterSpacing: "0.09em"
  title:
    fontFamily: "Playfair, PlayfairDisplay, Georgia, serif"
    fontSize: "clamp(26px, 3vw, 40px)"
    fontWeight: 500
    lineHeight: 1.15
    letterSpacing: "0.06em"
  body:
    fontFamily: "SourceSans3, SourceSansPro, system-ui, sans-serif"
    fontSize: "clamp(14px, 1.6vw, 24px)"
    fontWeight: 400
    letterSpacing: "0.09em"
  label:
    fontFamily: "SourceSans3, SourceSansPro, system-ui, sans-serif"
    fontSize: "16px"
    fontWeight: 400
    letterSpacing: "0.01em"
rounded:
  sm: "2px"
  card: "15px"
  full: "999px"
spacing:
  xs: "13px"
  sm: "24px"
  md: "40px"
  lg: "72px"
  xl: "99px"
components:
  button-primary:
    backgroundColor: "{colors.charcoal-brown}"
    textColor: "#FFFFFF"
    rounded: "{rounded.full}"
    padding: "12px 27px 12px 36px"
  button-primary-hover:
    backgroundColor: "{colors.charcoal-brown}"
    textColor: "#FFFFFF"
  button-secondary:
    backgroundColor: "#FFFFFF"
    textColor: "#000000"
    rounded: "{rounded.full}"
    padding: "12px 24px"
  tag:
    backgroundColor: "{colors.wisteria-bloom}"
    textColor: "#FFFFFF"
    rounded: "{rounded.full}"
    padding: "12px 28px"
---

# Design System: Bloom Up

## Overview

**Creative North Star: "The Collagen Bloom"**

Bloom Up is a collagen café and beauty bar in Mons' Grands Prés, built as the prototype for a future franchise network — brand decisions are made at that scale, not just for one site. The system reads as a physical extension of the product: soft, plump, nourishing shapes rendered in warm, sun-warmed color. Nothing has a sharp corner — buttons are full stadium pills, tags are rounded capsules, the hero's signature element is a literal spinning circle. Personality: **chaleureuse mais affirmée, accessible mais jamais banale, photogénique mais sincère** — a knowledgeable friend's voice, never an expert talking down or a shop pushing a sale. Headlines run in heavily-tracked uppercase; body copy stays lowercase.

The palette is warm and disciplined: Terracotta Bold is a full-bleed surface color used exactly twice per page — hero and footer, bookending everything between them — never a button or link. Wisteria Bloom (Electric Violet) is a single rare accent, at most one badge per section, never a background. A six-hue "complementary family" (Signal Red, Bright Lavender, Berry Pink, Ultramarine, Sunny Yellow, Acid Lime) exists for the brand at large — on the website they stay accent-only and under 2% of any page, but on other channels (print, merchandising, social) any one of them can become a full surface color.

**Key Characteristics:**
- Full stadium-pill buttons and tags; nothing sharp-cornered anywhere except the 2px keyboard-focus outline.
- Terracotta Bold is a bookend surface color (hero + footer only, exactly twice per page) — never a button, link, or repeated section fill.
- Flat by default — shadow appears only as a direct response to hover or a floating interaction, never as ambient card elevation.
- Three-family type system: Skinova for the hero headline only, Playfair for every other heading/label, Source Sans 3 for body copy, all heavily tracked.
- No page repeats a background color three sections in a row, and a secondary tone (Soft Nude, Rose Clay) appears at most once per page.

> **Implementation note:** this file documents the current target system (`.claude/skills/bloom-up-brand/SKILL.md`). `bloom-up-teaser.html` has been brought in line with it; `bloom-up-landing.html` (the main site) still runs the prior palette pending a follow-up pass — don't treat its live colors as authoritative until that update lands.

## Colors

The palette is warm and sun-lit, built around a strict "surface vs. accent vs. text" division so brand hues never leak into interactive elements.

### Primary
- **Terracotta Bold** (`#B45F52`): the brand's signature surface color, used as a full-bleed background exactly twice per page — the hero and the footer, bookending the content between them. Never a button, link, or a third section fill.

### Secondary
- **Wisteria Bloom / Electric Violet** (`#7047D7`): a single rare accent — at most one badge or pastille per section, never a background. See The One Accent Rule.
- **Soft Nude** (`#D8B8AE`) and **Rose Clay / Dusty Rose** (`#C88F86`): secondary section-background tones. Each appears at most once per page, and never on two consecutive sections back to back.

### Neutral
- **Warm Cream / Light Ivory** (`#F5EFEA`): the dominant neutral — roughly 55–60% of any given page.
- **Charcoal Brown** (`#1F1A18`): body text and every clickable control, site-wide. See The Neutral-Action Rule.
- **Espresso Brown / Dark Mocha** (`#4A352D`): reserved for menu item names/prices and category titles — a deliberately deeper, warmer dark than Charcoal Brown, used only in that context.
- **Warm Coral** (`#C96E5E`): a supporting shade, used sparingly alongside Terracotta.
- **Hairline** (`#E4D5CC`): the one divider/border tone — fine rules only, never a fill.

### Complementary Family (accent-only on the website; full surface color on other channels)
Signal Red (`#A90318`), Bright Lavender (`#9A70E8`), Berry Pink (`#D64F8C`), Ultramarine (`#4D5AC7`), Sunny Yellow (`#F2C84B`), Acid Lime (`#B8D34B`). On the site these stay under 2% of any page and never become a background — the same restraint as Wisteria Bloom. On print, merchandise, or social, any one of them may become a full surface color; that's channel-specific latitude the website itself doesn't take.

### Page Composition
A web page's color budget: ~58% Warm Cream, ~20% Terracotta (exactly twice — hero + footer), ~7.5% + 7.5% Soft Nude / Rose Clay (once each), ~5% text, ≤2% Wisteria Bloom / complementary accents. No background color repeats three sections in a row in a single scroll.

### Named Rules
**The Neutral-Action Rule.** Every interactive control — buttons, toggles, links, carousel arrows — is rendered in Charcoal Brown (or white on a dark surface), never in Terracotta, Wisteria Bloom, or any complementary hue. Brand and accent colors are surface and decoration only; they never carry a click target.

**The One Accent Rule.** Wisteria Bloom and the complementary family appear in at most one or two elements per section (a badge, a tag) and never as a section background or repeated UI fill.

**The Terracotta Bookend Rule.** Terracotta Bold is a full-bleed surface exactly twice per page — the hero and the footer — never a third time, and never a button or link color.

**The Two-Backgrounds Rule.** No page uses more than two background colors as full section fills at once (beyond the Terracotta bookends), always as flat blocks — no gradient, texture, or grain — and no color repeats for three consecutive sections.

## Typography

**Display Font:** Skinova (with Georgia, serif fallback)
**Headline/Title Font:** Playfair (with PlayfairDisplay, Georgia, serif fallback)
**Body Font:** Source Sans 3 (with SourceSansPro, system-ui, sans-serif fallback)

**Character:** An editorial pairing — a soft, rounded display serif reserved for a single hero moment, a second more classical serif carrying every other heading and label, and a warm, generously letter-spaced sans for body copy. Heavy tracking (0.09em) on body text is a deliberate brand signature — it's what gives the page its boutique, unhurried read even at small sizes.

### Hierarchy
- **Display** (400, `clamp(60px, 6.5vw, 104px)`, line-height 0.97): the hero headline only, once per page. Never reused elsewhere — see The Skinova Rule.
- **Headline** (500, 48px, uppercase, 0.09em tracking): section titles — Playfair, always uppercase.
- **Title** (500, `clamp(26px, 3vw, 40px)` down to 18px for smaller instances, 0.05–0.06em tracking): sub-headings within a section, menu item names and prices.
- **Body** (400, `clamp(14px, 1.6vw, 24px)`, 0.09em tracking): paragraph copy across the page.
- **Label** (400, 12–16px, uppercase where used, light tracking): nav links, button labels, small controls.

### Named Rules
**The Skinova Rule.** Skinova appears exactly once per page, on the hero headline only. It never sets a subheading, a label, or any other text — Playfair covers every other heading role.

**The Tracked-Type Rule.** Body and label text carry noticeably heavier letter-spacing (0.09em) than most web type, and it's never reduced to save space — a deliberate, consistent choice across the whole system.

## Layout

The page is a stack of full-bleed sections, each a flat color block (see Colors → Page Composition), separated by color change rather than a visible rule — a new background color at the section boundary *is* the divider. Vertical rhythm between content blocks runs on a five-step scale: 13px (photo grid gutters), 24px (heading → text), 40px (grid columns), 72px (between content blocks within a section), 99px (between sections). The horizontal page margin is a separate value that happens to share the 99px figure: 56px on narrow viewports, scaling fluidly to 99px from 1024px up to a 1920px design width, frozen above that.

## Elevation & Depth

The system is flat by default. There is no ambient card elevation anywhere — cards, tags, and photo grids sit directly on their section's background color with no shadow at rest. Depth between sections comes from color blocking, not layering.

### Shadow Vocabulary
- **Button hover-lift** (`box-shadow: 0 8px 24px rgba(35, 20, 9, 0.2)`, paired with `translateY(-2px)`): the only shadow a static element ever gains, and only on `:hover` of the primary CTA.
- **Floating menu preview** (`box-shadow: 0 18px 44px rgba(57, 25, 15, 0.26)`): a cursor-following product photo that appears on menu item hover — the system's one genuinely "lifted" object, and only while actively tracking the cursor.

### Named Rules
**The Flat-By-Default Rule.** Shadow is reserved strictly for direct-interaction feedback — never for passive elevation of a card, section, or badge. No `backdrop-filter` or blur anywhere in the system.

## Shapes

Two radii only, nothing in between: a full stadium/circle (buttons, tags, the "Voir plus" control, the spinning badge, carousel arrows) or a 15px card radius (menu cards, the floating menu-preview photo). The only sharp-cornered element on the entire page is the 2px-radius keyboard-focus outline.

### Named Rules
**The Two-Radii Rule.** A new element's border-radius is either fully rounded (stadium/circle) or exactly 15px (containers/cards) — there is no third option, and no small/barely-rounded corner anywhere.

## Components

### Buttons
- **Shape:** full stadium pill, height driven by 12px vertical padding.
- **Primary:** Charcoal Brown fill, white uppercase label. Always neutral — never Terracotta, never Wisteria Bloom.
- **Secondary/Ghost:** white fill, black uppercase label.
- **Hover/Focus:** primary lifts 2px with the hover shadow above; focus-visible gets a white 2px outline on dark/orange-toned surfaces.

### Tags / Badges
- **Style:** Wisteria Bloom fill, white text, fully-rounded pill, Playfair label type.
- **Use:** one or two per section maximum — see The One Accent Rule.

### Menu Card
- **Corner Style:** 15px radius.
- **Background:** white, no border, no resting shadow.
- **Internal Padding:** 28–32px, fine hairline rules between rows.

### Navigation
- **Style:** fixed, transparent over the hero, becomes solid Terracotta on scroll.

### Logo & Sunburst (signature component)
Four official lockups (wordmark + sunburst rays), one per approved background: Terracotta, Light Ivory, Dark Mocha, Electric Violet. A wordmark-only variant (white or dark, no rays) is reserved for off-system backgrounds — photography, the fixed nav. The sunburst is a core identity asset, not decoration: it's the one motif allowed to repeat freely across digital, the physical space, merchandise, and packaging — always the original artwork, never redrawn or recolored outside the palette, never with text overlaid directly on it.

### Iconography
No icon font, no third-party icon library. A single interface arrow (`arrow-discover.svg`), recolored/rotated via CSS mask (`background-color:currentColor` + `mask:url(...)`). The logo and the sunburst are the only other vector assets. No emoji-as-icon.

## Photography

Always color, never black-and-white, never a cold filter or gray studio backdrop. The primary set is the physical space itself — a handful of recurring corners of the café, built up into a visual signature over time. Mood: inspiring, energizing, appetizing, positive, creative. Stills are professionally shot and polished; video/reels can be looser but keep the same light and framing discipline.

## Do's and Don'ts

### Do:
- **Do** keep every button, tag, and small control fully rounded (stadium or circle), or exactly 15px for cards — see The Two-Radii Rule.
- **Do** use Charcoal Brown (or white on a dark surface) for anything clickable — see The Neutral-Action Rule.
- **Do** carry heavy letter-spacing (0.09em) on body and label text, never reduced to save space.
- **Do** reserve shadow for direct hover/interaction feedback only, never for resting elevation.
- **Do** use Terracotta Bold only for the hero and footer — exactly twice per page.

### Don't:
- **Don't** give Terracotta Bold, Wisteria Bloom, or any complementary hue to a button, link, or other click target.
- **Don't** repeat a background color three sections in a row, or use Soft Nude/Rose Clay more than once per page.
- **Don't** add a resting shadow to a card, badge, or container to make it feel "raised."
- **Don't** introduce a sharp or barely-rounded corner anywhere in the UI.
- **Don't** use Skinova anywhere except the single hero headline.
- **Don't** persist the mood-shuffle palette choice across visits — every fresh load starts on the default palette by design.
