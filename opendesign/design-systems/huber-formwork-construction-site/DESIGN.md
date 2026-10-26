# Huber Formwork — Construction Site

> Category: Industrial / Construction
> Surface: web

Signal-red formwork brand, sister to Huber Bau GmbH (Ravensburg). Formwork is the temporary structural mould into which concrete is poured — planks, walers, ties, props. The brand voice should feel like a well-run job site: precise, engineered, no decoration that does not earn its place. Sister-brand to Huber Bau: same paper/ink base, but signal red `#AD0C1B` replaces signal lime `#D8E84A`. When in doubt, look at what Huber Bau would do and swap the lime token for the red token.

## 1. Visual Theme & Atmosphere

Industrial editorial. The mood is a job site at 7am — first light on raw timber, concrete dust, a foreman marker pen. Type is heavy Archivo (geometric grotesque), almost brutalist but with Swiss precision. Mono labels in IBM Plex Mono. The red is not decorative — on a real formwork site, red waling beams and red safety markers are functional, not cosmetic. Treat the accent with the same seriousness.

Reference: think construction-site signage, engineering blueprints, Swiss railway typography, Perriand quietly used interior construction, but never trendy brutalist web.

## 2. Color

| Token | Hex | Use |
|---|---|---|
| `--hf-paper` | `#FAFAF7` | Page background, lightest surface |
| `--hf-paper-warm` | `#F5F4EF` | Card / hero wash gradient endpoint |
| `--hf-paper-soft` | `#F3F4E9` | Subtle tinted surface |
| `--hf-mineral` | `#EDEFDD` | Concrete/aggregate tint |
| `--hf-red` | `#AD0C1B` | Brand accent. Waling beams, key details, eyebrows, badge fills |
| `--hf-red-soft` | `#EBCFD2` | Red tint for hovers, low-emphasis red |
| `--hf-ink` | `#1A1A18` | Body / titles |
| `--hf-ink-2` | `#2A2A27` | Secondary ink |
| `--hf-mid` | `#5C5B53` | Tertiary text |
| `--hf-mid-2` | `#6F6E65` | Captions, mono labels |
| `--hf-mid-3` | `#8A897F` | Footer micro-copy |
| `--hf-line` | `#DEDDD5` | Hairline borders |
| `--hf-line-soft` | `#D3D4BE` | Construction-paper lines |
| `--hf-concrete` | `#C9C7BB` | Concrete / plywood face |

Accent discipline: Red is the only signal color. No orange, no lime. Use it sparingly: 3-4 touches per viewport (eyebrow square, waling beam in illustration, badge fill, link underline on hover). Never as a wash. Never as body text. Never below 12px height.

Selection: `background: #AD0C1B; color: #FAFAF7;`

## 3. Typography

- Archivo 400/500/600/700/800/900 — display + body (geometric grotesque, heavy weights do the work)
- IBM Plex Mono 400/500 — eyebrows, labels, technical readouts (engineering-blueprint voice)

Display clamp: `clamp(2.5rem, 4.6vw, 4.875rem)`
H2 clamp: `clamp(2.625rem, 4.6vw, 5rem)`
Body: 17px / 1.55 line-height
Mono caption: 11px / 0.15em letter-spacing / uppercase

Italic 900 on key nouns is encouraged (Linear-style editorial). Periods after fragments in mono labels (`bau. · ansicht. · gurtung.`).

## 4. Spacing

4-pt scale. Container max-width 1180-1320px. Hero card has 32-40px padding. Footer is tight (16-18px vertical). Construction-paper grid behind hero (faint vertical/horizontal hairlines at 100px intervals).

Border radius: 0 throughout. This is a job site, not a SaaS dashboard. Sharp corners and visible joints.

## 5. Layout & Composition

- Single-screen viewport-first hero (100vh, no scroll on desktop)
- Top brand wordmark centered, ~1.85rem
- Hero illustration 56vh max-height, centered, slightly offset left (-2rem) like a printed elevation drawing
- Bottom info card overlaps the hero illustration (~-80px), one accent rule on top, glass/blur backdrop
- Footer sticks to bottom, dark ink fill, brand left + impressum link right
- Mobile: card stacks 1-col, brand shrinks, footer stacks

## 6. Components

Wordmark — HUBER 900 + red bar (3px x 1.05em) + FORMWORK 400. The red bar is the visual handshake between the two sister brands (lime in Bau, red in Formwork).

Eyebrow — uppercase mono, 11px, letter-spacing 0.15em, leading 9px red square.

Info card — top border 3px red, padding 32-40px, 2-column grid (intro + contacts) on desktop, 1-column on mobile. Hairline dividers between contact rows.

Contact row — 112px label / 1fr value grid, mono label / Archivo value, red square bullets.

Footer — dark ink `#1A1A18`, paper-warm text, mono copyright left + impressum link right, link hover underline red.

## 7. Motion & Interaction

Construction-site restraint. Entrance is engineered — three chapters (sketch -> technical -> final) over ~9.5 seconds, autoplay once, then held.

- All hover transitions 200ms ease
- No bouncy easings, no spring physics
- Underline-on-hover for links (red)
- Reduced-motion: skip animation, hold final composition

## 8. Voice & Brand

German construction voice. Direct, technical, no marketing fluff. Words: Schalung (formwork), Gurtung (waling), Anker (tie), Stutze (prop), Schalhaut (form face), Elementstoss (panel joint). Headlines can be terse German: Wir schalen gerade um. or Demnachst verfugbar. Avoid anglicisms.

## 9. Anti-patterns

- Any other accent color (orange, lime, teal, blue)
- Gradients in red
- Rounded corners > 0
- Drop shadows > 4px blur
- Stock photography
- "We are coming soon" SaaS copy
- Three.js, WebGL, parallax scroll
- Gradient text, glowing buttons
- Using red as a section background
- Inter or Roboto (Archivo is non-negotiable)
