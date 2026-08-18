# Product

<!-- impeccable:product-schema 1 -->

## Platform

web

## Users

Primary: people already in or near the Grands Prés shopping gallery in Mons who stop in for a short, no-fuss self-care moment — grabbing a collagen drink, a coffee, or a quick LED skin treatment without dedicating a whole outing to it. *(Inferred from the site's copy and rituel framing — "sans y consacrer une journée," the 4-step rituel starting with "en arrivant" — not yet confirmed directly with Laurent; a clarifying round on this went unanswered.)*

## Product Purpose

Bloom Up is a collagen café & beauty bar: a single physical space that pairs a coffee/collagen-drink counter with an express beauty side (LED skin masks), so a visitor can care for their skin "from the inside" (the drinks) and "from the outside" (the treatment) in one relaxed stop. Success is a visitor leaving with, in the site's own words, "un glow naturel" — without it feeling like a spa visit or a medical appointment.

## Positioning

The differentiator is the combination itself, in one room: most collagen/wellness drink concepts are pure retail, and most LED/skin-treatment offerings are appointment-based beauty institutes. Bloom Up runs both from the same counter with two entrances off the gallery (café side / beauty side), letting a visitor cross over from one to the other on impulse rather than booking two separate destinations.

## Operating Context

- Location: Grands Prés shopping gallery, Mons, Belgium — accessible via two separate entrances from the gallery (one per side of the space).
- Not yet open: a second page in this repo (`bloom-up-teaser.html`, "Bientôt à Mons") is a pre-launch coming-soon page collecting sign-ups for the opening celebration. The main landing page's footer hours are an explicit "(à compléter)" placeholder for this reason — not a content gap to fill in speculatively.
- The rituel client is documented in 4 steps on the site: choose a treatment on arrival → settle into the cocooning space → LED mask → leave with a natural glow.
- Menu is organized into two categories so far: "Boissons Collagène" (signature collagen drinks, e.g. The Bloom, Rose Glow, Golden Bloom — ~9,50€ each) and "Café & autres boissons."

## Capabilities and Constraints

- Static site, no framework: a single self-contained HTML file per page (inline CSS/JS, no build step, no package manager). Confirmed by the repo — no `package.json` or bundler config exists.
- Menu photography and full opening hours are intentionally unfinished — Laurent doesn't have final business hours or per-product photography yet. Don't treat these as defects to fix proactively.
- The mood/palette "Shuffle my glow" toggle is a within-visit-only delight feature by design — it never persists a chosen palette across visits.

## Brand Commitments

- Name: **Bloom Up**. Tagline: **"Good inside. Glowing outside."**
- Voice: warm, boutique, a little playful — never clinical or overly medical/spa-formal, per the copy's tone throughout ("un lieu doux," "sans y consacrer une journée").
- Visual identity is fully specified in [DESIGN.md](DESIGN.md) (Creative North Star: "The Collagen Bloom") — that file is the source of truth for palette, type, and component language; this file stays product-only.

## Evidence on Hand

- Real menu copy and pricing exist on the live page for the "Boissons Collagène" category (item names, descriptions, and prices in €) and photography for Concept/Espace sections.
- No confirmed opening date, social media handles, or exact street address beyond "Grands Prés, Mons" — do not invent these; the teaser page's sign-up form is the only evidence of pre-launch status.
- Footer hours are a known placeholder, not a fact to fabricate.

## Product Principles

1. **One space, two entries, one visit.** Never design the café and beauty sides as if they were separate businesses that happen to share a wall — the crossover between them is the whole point.
2. **Self-care without ceremony.** Every product and flow decision should protect the "quick, no-fuss" framing — a visitor should never feel like they've booked a spa appointment.
3. **Don't fabricate what isn't final.** Hours, product photography, and any launch-date/social details are explicitly unresolved; treat placeholders as intentional, not as bugs to quietly fill in.
4. **The rituel is the product's plain-language pitch.** The 4-step arrival→settle→treatment→glow sequence is the simplest expression of what Bloom Up does — new copy or flows should stay legible against it.
