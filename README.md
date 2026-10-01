# Orbio bit field

Animated 0101 grid for Orbio backgrounds. The tinted cells stay fixed; only the 0s and 1s change.

- **Fields:** Stone (background base), Vein, Celeste, Brass, Void (dark), Vein CTA (calm centre for a headline)
- **Motion:** Flicker, Wave, Stream; the pointer stirs nearby digits
- **Keys:** `H` hides the controls (for screen recording), `Space` pauses
- Respects `prefers-reduced-motion` (opens paused)

Grid: 40px cells, Geist Mono 20px digits, one tint level per cell. Every row spells "ORBIO " in 8-bit ASCII.
At 1920×1080 it matches the Figma masters cell for cell (ASSETS → "BIT FIELD" in the ORBIO file).
The field data comes from `tools/patterns/bitfield.py` in the brand project.

Static single file: `index.html`, no build step.

## Hero mockups (Home + Launchpad + Protocol)

`protocol-hero/` holds both sub-brand heroes on a dimmed 20px bit field. Text blocks knock the field out on whole cells.

- **Home** (`#home`, or `home-hero/`): ORBIO master lockup (2 grid cells tall), Vein accent, the Buy credits card, marble Hypatia; same layout as the other views
- **Protocol** (`#protocol`): ORBIO MARKETPLACE lockup, Brass, marble hand holding CREDIT
- **Launchpad** (`#launchpad`, or `launchpad-hero/`): ORBIO LAUNCHPAD lockup, Celeste, marble Apollo raising the orb

Marble is the default variant; Void is the dark one. The switch sits bottom-right (`H` hides it). Copy is verbatim from orbio.so.

### Reveal variant (no full-width grid)

`protocol-hero/reveal.html` is the same four heroes without the full-width field. The bits rest faintly around each statue, and the cursor wakes them as it moves: they light up with their grid square, sometimes flip, and fade within about 1.5 s, leaving a trail. No knock-out boxes, no drop shadows. Shortcuts: `home-reveal/`, `launchpad-reveal/`, `protocol-reveal/`, `incognito-reveal/`. The original flowing-field version stays at `protocol-hero/` for comparison.

The headlines and wordmark are outlined from ABC Arizona Flare (Dinamo trial). License it before production use.
