# Ginrin Sanctuary · Project goal

Build a welcoming, beautiful, playable koi genetics and hatchery-management game **inspired by** Koi Farm, but with original visual assets and code. Preserve the calm collecting/breeding experience while making navigation, sorting, and fish inspection effortless.

## Desired play loop

1. New wild-type koi enter from a waterfall-fed stream as a baseline breeding population.
2. Select visually attractive fish for the main sanctuary or breeding channel.
3. Breed fish to discover inherited pigments, patterns, finishes and rare new morphs.
4. Fry pass through adjustable one-way slatted/weir passages into nursery or holding tanks, subject to a meaningful age/size rule.
5. Sort mature fish among four or five classification areas, compare lineages, and return favorites to the showcase pond.
6. Inspect fish up close, emphasizing lifelike movement, vibrant color, and reflective Ginrin scales when lifted for transfer.
7. Preserve game progress locally and import/export collections and lineage as JSON.

## Product priorities

- A smooth **scrollable and pannable watercourse map** with physically visible connections between ponds and tanks.
- **Friendly visual and interaction design** that does not conceal the fish under persistent technical HUDs.
- Clear interaction patterns for mouse, touch, and keyboard, with accessible instructions and recoverable drag operations.
- Progressive quality tiers: quick Canvas fallback, WebGL/Three.js visuals where supported, user-controlled quality settings, graceful low-power mode.
- Gentle, explainable progression; rare morphs should be elusive, with configurable rarity/population equilibrium rather than unbounded spawning.
- Document real-world koi classifications separately from fantasy or stylized cosmetic morphs.

## Acceptance criteria for next iteration

- Game loads without runtime errors and can be played using mouse and touch.
- Fish remain confined to visible water areas; transfers never strand or silently lose fish.
- A breeding pair yields identifiable offspring with persistent parents and trait data.
- Juveniles only traverse an **open and eligible** one-way gate; adults are blocked by size rules.
- Nursery/holding occupancy and stream population update reliably.
- Saved state survives reload; an exported JSON file can be imported into a new browser session.
- Three.js migration begins with one representative koi and a shader demonstration, without sacrificing the usable fallback.

## Important implementation distinctions

**Prototype as of 2026-10-17:** the refined `index.html` is a Canvas 2D single-file game with simplified inheritance and schematic routing. Do not claim it already contains Three.js, real hydrological physics, measured fish dimensions, or scientifically correct Mendelian genetics.

Never use Koi Farm artwork, source code, or trademarked game branding as assets. It is a gameplay reference, not a dependency.
