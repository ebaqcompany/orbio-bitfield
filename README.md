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

## Hero sections (Home + Launchpad + Protocol + Incognito)

Four Orbio website heroes in one page: `protocol-hero/reveal.html`. Switch between them from the navbar, or open one directly:

- **Home:** `home-reveal/`, ORBIO master lockup, Vein accent, the Buy credits card, marble philosopher
- **Launchpad:** `launchpad-reveal/`, ORBIO LAUNCHPAD lockup, Celeste, marble Apollo raising the orb
- **Protocol:** `protocol-reveal/`, ORBIO MARKETPLACE lockup, Brass, marble Hypatia
- **Incognito:** `incognito-reveal/`, ORBIO INCOGNITO lockup, Iris, veiled marble statue

The 20px bit grid is invisible: only its 0s and 1s show. They rest faintly around each statue, and the cursor wakes them anywhere on the hero (they light up, sometimes flip, and fade within about 1.5 s). Hairlines on the grid mark the layout: two rails 40px in from the edges, a line under the 80px nav band, and two guide rails bracketing the copy. `H` hides the controls. Copy is verbatim from orbio.so.

The headlines and wordmark are outlined from ABC Arizona Flare (Dinamo trial). License it before production use.
