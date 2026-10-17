# Ginrin Sanctuary · Living Waters

A local-first koi collecting and breeding prototype, refined from the user's Gemini-generated **Ginrin Sanctuary** HTML experiment. This is a separate project within the `spawn` repository.

## Run it

Open [index.html](./index.html) directly in Chrome, Edge, or another modern browser. No build tool or external dependencies are needed.

## Included in this prototype

- Pannable, zoomable hatchery with mountain stream, main pond, breeding channel, nursery, and four holding tanks.
- Fish selection and transfer by drag or dropdown.
- Procedurally colored and animated koi with scale shimmer.
- Simplified offspring generation, parent references, and automatic fry-gate movement.
- Collection / specimen inspection.
- Automatic browser-local saves, JSON export and JSON import.
- Responsive small-screen layout.

## Status and boundaries

- **Renderer:** HTML5 Canvas 2D, **not** Three.js or real WebGL shaders yet.
- **Genetics:** simplified game rules, not a scientifically validated koi genetic model.
- **Hydraulics:** illustrated channels / gate passage; not a physically correct water-flow or slat-size simulation.
- **Persistence:** localStorage and manual JSON exports; no cloud synchronization.
- **Validation:** JavaScript passed a syntax check. Interactive play and cross-browser behavior need dedicated testing.

## Development handoff

Read [PROJECT_GOAL.md](./PROJECT_GOAL.md) for user intent and acceptance criteria and [AGENTS.md](./AGENTS.md) before editing. Original Gemini V1 is preserved under [reference/](./reference/).

Start with an actual browser smoke test of the existing game, then fix any discovered input, drawing, resize, transfer, save/load, or accessibility bugs. Keep a working standalone build while adding Three.js gradually.
