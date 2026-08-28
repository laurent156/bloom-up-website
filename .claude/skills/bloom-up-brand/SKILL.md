---
name: bloom-up-brand
description: Bloom Up's official brand and design system — colors, typography, spacing, shapes, motion, components, and the never-break brand rules. Use for any design or visual work on Bloom Up (web, print, merch, social) to stay on-brand. Authored by Laurent as the franchise-scale source of truth; supersedes ad-hoc values found in existing code.
user-invocable: true
---

# Bloom Up — Design Skill

Bar à boissons au collagène doublé d'une dimension beauté accessible. Hybride café lifestyle / institut. Ouverture automne 2026, Mons (Grands Prés, Belgique). Conçu comme le prototype d'un réseau de franchises — les décisions de marque se prennent à cette échelle. Toute la marque parle français (marché belge/Mons).

**Valeurs :** Vitalité, Partage, Modernité, Authenticité. **Personnalité :** chaleureuse mais affirmée, accessible mais jamais banale, photogénique mais sincère. Voix : phrases courtes, déclaratives, une amie qui s'y connaît — jamais une experte qui surplombe ni une boutique qui pousse à l'achat. Titres en majuscules très tracées ; corps de texte en minuscules. Pas d'emoji dans le ton de marque, à l'exception ponctuelle du ✦.

## Couleurs

**Marque**
- Terracotta Bold `#B45F52` — surface pleine (héros + pied de page), jamais un bouton ni un lien.
- Wisteria Bloom / Electric Violet `#7047D7` — accent unique, une pastille/badge par section max, jamais un fond.
- Espresso Brown / Dark Mocha `#4A352D` — noms/prix de menu, titres de catégories.

**Secondaires — une fois par page, jamais deux sections consécutives**
- Soft Nude `#D8B8AE`
- Rose Clay / Dusty Rose `#C88F86`

**Neutres & texte**
- Warm Cream / Light Ivory `#F5EFEA` — dominante, ~55–60% de chaque page.
- Charcoal Brown `#1F1A18` — texte courant et tout contrôle cliquable.
- Warm Coral `#C96E5E` — nuance de soutien.
- Hairline `#E4D5CC` — filets fins uniquement.

**Famille complémentaire (accent-only sur le site — badge/pastille, jamais un fond, ≤2% d'une page ; sur les autres supports — print, merch, réseaux — chacune peut devenir couleur de surface)**
Rouge Signal `#A90318`, Bright Lavender `#9A70E8`, Berry Pink `#D64F8C`, Ultramarine `#4D5AC7`, Sunny Yellow `#F2C84B`, Acid Lime `#B8D34B`.

**Répartition d'une page web :** ~58% Warm Cream, ~20% Terracotta (exactement 2×: héros + footer), ~7,5%+7,5% Soft Nude/Rose Clay (1× chacune), ~5% texte, ≤2% accent violet/complémentaire. Aucune couleur ne se répète 3× de suite dans un scroll.

## Typographie — trois familles, un rôle chacune

- **Skinova** (display serif) — titre héros uniquement, une seule fois par page. `clamp(60–104px)`, line-height 0.97.
- **Playfair** — tous les titres, labels, pastilles, noms de menu. Toujours tracking large (0.02–0.09em), souvent majuscules.
- **Source Sans 3** — tout le corps de texte, tracking 0.09em (signature de la marque : donne l'allure boutique/non pressée).

Jamais Inter/Roboto/autre famille tierce. Ne jamais réduire l'interlettrage pour gagner de la place.

## Espacement & mise en page

Blocs pleins empilés ; on change de section en changeant de couleur de fond, jamais avec un trait ou une ombre.
- Space XS 13px — gouttière grille photo
- Space SM 24px — titre → texte
- Space MD 40px — colonnes de grille
- Space LG 72px — entre blocs de contenu
- Space XL 99px — entre sections

Marge de page : 56px mobile → 99px fluide dès 1024px, figée au-delà de 1920px.

## Formes & ombres

Deux rayons seulement, rien entre les deux : pilule/cercle complet (boutons, pastilles, flèches, badge tournant) ou carte 15px (cartes, photo flottante). Seul angle vif : le contour de focus 2px.

Pas d'ombre au repos — la profondeur vient du fond coloré. Ombre uniquement en feedback d'interaction : lift bouton primaire au survol `0 8px 24px rgba(35,20,9,.2)`, photo de prévisualisation qui suit le curseur `0 18px 44px rgba(57,25,15,.26)`. Pas de `backdrop-filter`/flou.

## Iconographie

Aucune police d'icônes, aucune bibliothèque tierce. Une seule flèche d'interface (`arrow-discover.svg`), recolorée/pivotée par masque CSS (`background-color:currentColor` + `mask:url(...)`). Logo et sunburst sont les seuls autres vecteurs. Pas d'emoji-icône.

## Logo & Sunburst

Quatre déclinaisons officielles (wordmark + rayons sunburst), une par fond approuvé : Terracotta, Light Ivory, Dark Mocha, Electric Violet. Wordmark seul (`logo-bloom-up-white.svg` / `-dark.svg`, sans rayons) réservé aux fonds hors système (photo, nav fixe).

Le sunburst est un actif d'identité central — pas un simple décor du site — et le seul motif autorisé à se répéter librement (digital, architecture du point de vente, merchandising, packaging). Toujours le dessin d'origine, jamais redessiné ni recoloré hors palette ; jamais de texte superposé directement.

## Photographie

Toujours en couleur, jamais N&B, jamais de filtres froids ni fond gris studio. Décor principal : le lieu lui-même — quelques coins récurrents du café pour bâtir une signature visuelle. Mood : inspirant, énergisant, gourmand, positif, créatif. Photo pro et soignée ; vidéo/reels moins léchée mais lumière et cadrage tenus.

## Mouvement

Deux régimes : ambiance lente et continue (badge héros 30s, ticker 48s, reveals scroll 600–900ms en `ease-out-quart`/`ease-out-expo`) vs interaction brève et nette (150–350ms, bouton primaire lift 2px + ombre chaude puis retour à plat). Jamais de spring/élastique/rebond nulle part.

## Composants

- **Bouton** — primaire (pilule sombre, blanc dessus) / ghost (pilule blanche). Toujours neutre — jamais terracotta, jamais violet.
- **Badge** — pastille Wisteria Bloom, catégorie/statut, 1–2 par section max.
- **Carte menu** — fond blanc, rayon 15px, sans bordure ni ombre au repos, padding 28–32px, filets fins entre lignes.
- **Barre de navigation** — fixe, transparente sur le héros puis pleine Terracotta au scroll.

## Règles clés à ne jamais enfreindre

1. **Neutral-Action** — tout élément cliquable est en Charcoal Brown ou blanc sur fond sombre, jamais dans une couleur de marque.
2. **One Accent** — Wisteria Bloom (et la famille complémentaire) ne devient jamais un fond de section ni une couleur d'interface répétée.
3. Terracotta = surface pleine en bookend uniquement (héros + footer), jamais bouton/lien.
4. Deux couleurs de fond max par page, en blocs pleins — pas de dégradé, texture, grain.
5. Skinova : héros uniquement, jamais ailleurs.
