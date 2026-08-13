---
name: Bloom Up
description: Collagen café & beauty bar in Mons, Grands Prés — warm, editorial, pill-shaped everywhere
colors:
  sunrise-orange: "#F16925"
  wisteria-bloom: "#A790EA"
  warm-cream: "#FBF4EA"
  blush-rose: "#FDE8E9"
  buttercream: "#FFEBC6"
  charcoal-brown: "#353535"
  espresso-brown: "#39190F"
  dusty-rose: "#DF90A6"
  warm-nude: "#C8B4A4"
  muted-nude: "#B0A090"
  terracotta-shadow: "#8B6565"
  hairline: "#E8E0D8"
  hairline-soft: "#F0EBE4"
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
  md: "15px"
  lg: "30.5px"
  full: "37px"
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
    rounded: "{rounded.lg}"
    padding: "12px 28px"
---

# Design System: Bloom Up

## Overview

**Creative North Star: "The Collagen Bloom"**

Bloom Up is a collagen café and beauty bar in Mons' Grands Prés, and its whole visual system reads as a physical extension of the product: soft, plump, nourishing shapes rendered in warm, sun-warmed color. Nothing on this page has a sharp corner — buttons are full stadium pills, tags and badges are rounded capsules, the hero's signature element is a literal spinning circle, and even the section-to-section rhythm favors generous, unhurried padding over tight grids. The mood is **warm & refined**: editorial serif headlines and a composed, boutique-café restraint lead, with a bright terracotta-orange and a candy-soft pastel purple supplying the warmth and personality underneath.

The palette is anchored by Sunrise Orange as a full-bleed surface color (hero, ticker, footer), not as an interactive accent — see the Named Rule under Colors. Wisteria Bloom, a soft pastel purple, is reserved for small badge/tag moments and the hero's rotating signature badge. Everything else is warm neutrals: creams, blushes, and two distinct dark browns that split duty between primary text (Charcoal Brown) and menu/heading emphasis (Espresso Brown).

Depth is conveyed through color blocking between full-bleed sections, not through shadows or layering — the system is flat at rest, with shadow reserved for two specific interaction moments (see Elevation & Depth). Motion is quiet and ambient by design intent (a deliberate "slow it down" pass already ran on the hero's ticker and badge spin), while direct interactions (button hover, menu reveal) stay snappy.

**Key Characteristics:**
- Full stadium-pill buttons and badges; nothing sharp-cornered anywhere in the system.
- Sunrise Orange is a surface/section color, never a button color — interactive actions are always the dark neutral.
- Flat by default — shadow appears only as a direct response to hover or a floating interaction, never as ambient card elevation.
- Three-family type system: a display serif for the hero headline only, a distinct serif for all other headings/labels, and a warm sans for body copy.
- Warm neutrals (cream, blush, buttercream) carry most of the page; the two brand hues (orange, purple) are used sparingly and deliberately.

## Colors

The palette is warm and sun-lit throughout — no cool grays, no pure black or white anywhere except white button/card fills.

### Primary
- **Sunrise Orange** (`#F16925`): the brand's signature surface color — full-bleed background for the hero, the ticker/marquee bar, and the footer. Never used as a button or link color; see the Neutral-Action Rule below.

### Secondary
- **Wisteria Bloom** (`#A790EA`): a soft pastel purple reserved for small, deliberate moments — the hero's spinning circular badge and small category/tag pills (`.badge-green`, `.badge-outline-green`). Always paired with white text.

### Tertiary
- **Buttercream** (`#FFEBC6`): the section-background color for La Carte and the Rituel content panel — a warm, buttery cream distinct from the page's base cream, used to block out whole sections rather than as an accent.
- **Blush Rose** (`#FDE8E9`): the section-background for L'Espace, and doubles as a light/pale tint elsewhere on orange surfaces.

### Neutral
- **Warm Cream** (`#FBF4EA`): the page's base background color (`body`).
- **Charcoal Brown** (`#353535`): primary text color and the fill for every interactive button — see the Neutral-Action Rule.
- **Espresso Brown** (`#39190F`): a deeper brown than Charcoal, used specifically for menu item names/prices/category titles and the Espace body copy — the system deliberately uses two distinct dark browns for different emphasis levels.
- **Dusty Rose** (`#DF90A6`): menu item description text — a warmer, more saturated tone than the pale Blush Rose surface tint, kept legible against white menu cards.
- **Warm Nude** (`#C8B4A4`) / **Muted Nude** (`#B0A090`): fallback background colors behind the hero photo and photo-cards respectively, shown only while an image is loading.
- **Terracotta Shadow** (`#8B6565`): fallback background behind the Rituel image.
- **Hairline** (`#E8E0D8`) / **Hairline Soft** (`#F0EBE4`): the two divider/border tones used in the menu grid and card borders.

### Named Rules
**The Neutral-Action Rule.** Every interactive control — both hero CTAs, the shuffle toggle, the Carte carousel arrows, "Voir plus" — is rendered in Charcoal Brown (or white on an orange surface), never in Sunrise Orange or Wisteria Bloom. The brand hues are surface and decoration colors; they never carry a click target.

**The One Accent Rule.** Wisteria Bloom appears in at most one or two elements per section (the badge, a tag). It never becomes a section background or a repeated UI color — its rarity is what keeps it feeling special rather than decorative wallpaper.

## Typography

**Display Font:** Skinova (with Georgia, serif fallback)
**Headline/Title Font:** Playfair (with PlayfairDisplay, Georgia, serif fallback)
**Body Font:** SourceSans3 (with SourceSansPro, system-ui, sans-serif fallback)

**Character:** An editorial pairing — a soft, rounded display serif reserved for a single hero moment, a second more classical serif carrying every other heading and label, and a warm, generously letter-spaced sans for body copy. The heavy tracking on nearly all body and label text (0.09em+) is what gives the page its boutique, unhurried read even where the type is small.

### Hierarchy
- **Display** (400, `clamp(60px, 6.5vw, 104px)`, scaling to 146px at desktop widths, line-height 0.97): the hero headline only ("Good inside. Glowing outside."). Never reused elsewhere.
- **Headline** (500, 48px, uppercase, 0.09em tracking): section titles ("La Carte", "L'Espace", "Le Rituel") — Playfair, always uppercase, always this exact weight/tracking.
- **Title** (500–600, `clamp(26px, 3vw, 40px)` down to 18px for smaller instances, 0.05–0.06em tracking): sub-headings within a section — the Rituel heading, menu item names and prices.
- **Body** (400, `clamp(14px, 1.6vw, 24px)`, 0.09em tracking): paragraph copy across the page (hero subhead, Espace/Rituel body text, menu item descriptions).
- **Label** (400, 12–16px, uppercase where used, light tracking): nav links, the "Voir plus" control, button labels.

### Named Rules
**The Tracked-Type Rule.** Body and label text carry noticeably heavier letter-spacing (0.09em) than most web type. This is a deliberate, consistent choice across the whole system — new body copy should match it rather than defaulting to normal tracking.

## Layout

The page is a stack of full-bleed sections, each with its own background color block (see Colors → Tertiary/Neutral), separated by generous top padding (72–113px) rather than visible rules — color changes at the section boundary *are* the divider. A horizontal page margin (`--page-x`) holds 56px on narrower viewports and scales fluidly to 99px from 1024px up to a 1920px design width, after which it freezes (the system's one deliberately Figma-pixel-precise fluid-scale token — see the sidecar for the exact technique). Breakpoints sit at 767px (mobile), 1023px (tablet), and 1439/1440px (the point where several sections switch from a responsive flex/grid layout to Figma-precise absolute geometry — notably the hero, which is structurally incompatible with pixel-exact positioning below that width).

Grids stay tight and deliberate: a 13px gutter on full-bleed photo rows (Concept, Espace), a 40px column gap on the two-column menu grid. Section content itself is comfortably wide — body copy rarely exceeds ~470–650px per column even on a full-bleed section, keeping reading measure short despite the generous canvas.

## Elevation & Depth

The system is flat by default. There is no ambient card elevation anywhere — cards, tags, and photo grids sit directly on their section's background color with no shadow at rest. Depth between sections comes from color blocking, not layering.

### Shadow Vocabulary
- **Button hover-lift** (`box-shadow: 0 8px 24px rgba(35, 20, 9, 0.2)`, paired with `translateY(-2px)`): the only shadow a static element ever gains, and only on `:hover` of the primary CTA. Removed again on `:active`.
- **Floating menu preview** (`box-shadow: 0 18px 44px rgba(57, 25, 15, 0.26)`): a cursor-following product photo that appears when hovering a menu item — the system's one genuinely "lifted" object, and it only exists while actively tracking the cursor.

### Named Rules
**The Flat-By-Default Rule.** Shadow is reserved strictly for direct-interaction feedback (a hover-lift, a floating cursor-follower) — never for passive elevation of a card, section, or badge. If a new component seems to need a resting shadow to feel "raised," reconsider the component instead of adding the shadow.

## Shapes

Every corner in the system is either fully rounded (buttons, tags, the "Voir plus" control, the spinning badge, the carousel arrow controls — all rendered as stadiums or circles regardless of the exact radius value used to achieve it) or a soft 15px card radius (menu cards, the floating menu-preview photo). The only sharp-cornered element on the entire page is the 2px-radius focus-visible outline used for keyboard accessibility — everything else avoids right angles entirely.

### Named Rules
**The No-Sharp-Corners Rule.** If a new element needs a border-radius, default to either a full stadium/circle (interactive controls, tags) or 15px (containers/cards). A sharp or barely-rounded corner reads as off-brand immediately.

## Components

### Buttons
- **Shape:** full stadium pill (`border-radius: 37px`), height driven by 12px vertical padding rather than a fixed height.
- **Primary** (`.btn-dark`): Charcoal Brown fill, white uppercase label, asymmetric padding (36px leading / 27px trailing) that reserves room for a trailing arrow icon.
- **Secondary/Ghost** (`.btn-ghost`): white fill, black uppercase label — used for the lower-emphasis CTA sitting beside the primary one.
- **Hover/Focus:** primary lifts 2px with the hover shadow above; focus-visible gets a white 2px outline (vs. the system default dark outline) since it sits on a dark/orange surface.

### Tags / Badges
- **Style:** Wisteria Bloom fill, white text, ~30.5px radius pill, Playfair label type.
- **Use:** category or status tags on photo cards and the Rituel heading — never more than one or two per section (see The One Accent Rule).

### Cards / Containers
- **Corner Style:** 15px radius (14px at tablet).
- **Background:** white (menu cards) or a fallback nude/terracotta tone shown only while its photo loads.
- **Shadow Strategy:** none at rest — see Elevation & Depth.
- **Internal Padding:** 32px/28px (menu cards).

### Navigation
- **Style:** fixed, transparent over the hero, uppercase 16px white links with an opacity-fade hover; becomes a solid orange bar with a hamburger-driven dropdown below 1024px.
- **Signature control:** the "Shuffle My Glow" mood toggle — an outlined pill (not a solid CTA-weight fill, deliberately de-emphasized below the two real CTAs) that reassigns which of the brand's 5 approved colors plays which role, reset to the default Sunrise palette on every fresh visit rather than persisted.

### Menu Hover Preview (signature component)
A cursor-following floating photo (260×300px, 15px radius, the system's one true drop shadow) that appears next to the cursor when hovering a menu item name with a configured photo, replacing the cursor itself while active. The clearest expression of "playful but grounded" in the whole system — a delight moment scoped to exactly one interaction.

## Do's and Don'ts

### Do:
- **Do** keep every button, tag, and small control fully rounded (stadium or circle) — see The No-Sharp-Corners Rule.
- **Do** use Charcoal Brown (or white on a dark surface) for anything clickable — see The Neutral-Action Rule.
- **Do** carry heavy letter-spacing (0.09em) on body and label text to match the system's tracked-type character.
- **Do** reserve shadow for direct hover/interaction feedback only, never for resting elevation.
- **Do** use Sunrise Orange only as a full-bleed section background, never as a small accent or button fill.

### Don't:
- **Don't** give Sunrise Orange or Wisteria Bloom to a button, link, or other click target.
- **Don't** add a resting shadow to a card, badge, or container to make it feel "raised" — block color and section rhythm carry depth instead.
- **Don't** introduce a sharp or barely-rounded corner anywhere in the UI.
- **Don't** persist the mood-shuffle palette choice across visits — every fresh load starts on the default Sunrise palette by design.
