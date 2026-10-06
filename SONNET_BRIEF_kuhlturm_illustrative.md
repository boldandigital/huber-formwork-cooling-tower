Prompt for Sonnet (copy everything below the line into claude.ai or the ultracode wrapper):

---

HUBER FORMWORK v2 — Kühlturm redesign brief

We're pivoting the cooling tower (Kühlturm) hero illustration from a literal 10-takt Kletterschalung construction sequence to a more illustrative, editorial concept. The current animation feels too technical and literal — it shows the actual building process (concrete pouring, rebar, curing) which is accurate but reads more like an engineering diagram than a brand illustration.

New direction — Kühlturm as a finished object being wrapped/dressed:

The cooling tower should be illustrated as a complete, finished hyperboloid silhouette (a recognizable cooling tower shape — narrow throat in the middle, wider at the base and the lip at the top). The shape is static from the start, drawn clean and editorial like an architectural rendering on the warm paper background (#FAFAF7).

Around the tower, a continuous ribbon / sleeve / wrap of freshly-cast concrete panels moves from left to right, wrapping around the tower like a banner or a bandage being applied. The wrap could be made of:
- A series of rectangular concrete panels (Betonplatten) that flow across the silhouette in sequence, each one settling into place as it passes around the curve
- OR a single continuous ribbon that unfurls, wraps around the tower once or twice, and trails off
- OR a wave/stream of individual concrete plates that arc around the tower and stack against it as they pass

The motion is left-to-right, smooth, flowing — not jerky like a construction timeline. Think of how a film credits sequence wraps text around a 3D object, or how a long banner flows in the wind and lands on a column. The panels are the same warm-grey concrete gradient as before (#A8A89E → #C9C7BB → #A8A89E), with thin ink outlines, on the paper background.

The reference style is the editorial construction-drawing aesthetic of the Huber Bau / v1 deckenschalung page (which uses Archivo display type, IBM Plex Mono labels, signal red #AD0C1B accent, hand-drawn-feeling line work, technical-drawing feel with dimensions and labels). The Kühlturm should look like an editorial illustration of the finished product, not a construction process diagram.

The chapter labels can still cycle (01 EINSCHALEN & BEWEHREN → 02 BETONIEREN IM TAKT → 03 AUSSCHALEN) but the chapter transitions should happen as the wrap completes its pass, not as discrete construction events. The wrap IS the chapter sequence, told as one continuous motion.

Keep:
- 1200×600 viewBox, paper background, construction-paper grid
- Editorial construction-drawing feel
- Signal red (#AD0C1B) as the accent — used for the wrap's leading edge / active panel, the chapter labels, the dimension callouts, the crane
- The H=150m vertical dimension on the right, Ø=76m horizontal dimension at the throat, 25m scale bar at the bottom, Takt counter
- The crane silhouette (mast + jib + counterweight + swinging red bucket) climbing at the top
- Steam plumes rising from the top after the wrap completes
- Approx 10s total runtime
- Mobile responsive (max-height 56vh on small screens)

Remove or rethink:
- The literal concrete pour (scaleY 0→1) and cure (brightness) animations — these are what makes it feel like a build sequence
- The rebar starter bars
- The progressive formwork yokes being added/removed
- The 10-takt stepped timeline

The wrap motion is what tells the story. The tower is the canvas, the wrap is the action.

Please write the full self-contained HTML/CSS/JS as a single code block I can paste into the existing v2 page (it has a `<div id="hf-stage-inner">` and a `<svg class="hf-hero__svg">` that I want to replace). Keep the wordmark, info card, and footer markup — only swap the SVG body, the SVG-specific CSS, the keyframes, and the inline script. Don't touch the surrounding HTML structure.

Also: don't render the chapters as 3 separate fading labels. Render them as a single persistent label that updates as the wrap progresses, OR render all 3 stacked and just fade the inactive ones. The current cycling feels too presentation-like.
