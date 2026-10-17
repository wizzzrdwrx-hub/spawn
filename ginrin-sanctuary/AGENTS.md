# Codex instructions · Ginrin Sanctuary

You are working **only in `ginrin-sanctuary/`** unless specifically directed otherwise. The sibling projects and root README belong to other work; do not modify them. The immediate objective is to evolve the working prototype into a refined koi game, not to rewrite unrelated infrastructure.

## Start here

1. Read `PROJECT_GOAL.md`, `README.md`, and `index.html`.
2. Establish a working browser run and capture current interactions.
3. Run JavaScript syntax checks and test important user flows before major refactors.
4. Save/commit small changes with a short summary of behavior verified and known limitations.

## First engineering assignment

Implement and test the **smallest reliable gameplay foundation** before replatforming rendering:
- Reliable pointer/touch selection, dragging, panning, and drop-target feedback.
- Stable coordinate transforms and resize/zoom handling.
- Explicit fish spatial placement when transferring and after import.
- Deterministic and inspectable breeding state, unique offspring IDs, parent lineage, and gate eligibility.
- UI feedback for full tanks, invalid transfers, gate states, and failed saves.
- Defensive JSON parsing, schema versioning, and migration strategy.

Then prototype a **Three.js koi renderer** with a single animated fish, a simple iridescent/metallic material, and a graceful Canvas fallback. Avoid adding mandatory CDNs or network services to the current offline single-file build without an intentional packaging solution.

## Practical verification

For static JS syntax checks, extract the inline script from `index.html` and run `node --check` on it. Use a real browser to verify animation, layout, transfers, spawn, save, reload, export, import, touchscreen input, and responsive layouts. Syntax checks alone are insufficient.

## Safety and provenance

- Preserve the current HTML as a runnable baseline while implementing changes.
- The source file `reference/gemini-v1.html` is archival; do not edit.
- Distinguish simulated mechanics from validated aquarium physics and genetics.
- Do not include user private information in public commits.
- Keep assets original and respect third-party game copyright.
- Do not claim tests passed unless you actually ran them.
