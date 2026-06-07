# Tiny Reactions

A single-page interactive toy. Drag two elements into the reaction zone and watch them
become something real — water, salt, rust, diamond. Hover (or tap) anything for a one-line
fun fact. A discovery log tracks the 13 compounds you can find.

It's **curated, not simulated** — the eleven elements, thirteen reactions, and two
non-reactive noble-gas gags are all hardcoded data. No chemistry engine.

## Design

Crayon-on-sketchbook-paper aesthetic that still feels premium: hand-drawn wobbly blobs,
marker handwriting (Shantell Sans), and a reaction for every action — hover, drag, drop,
and a distinct reveal animation for each of the 13 compounds.

## Run it

It's one self-contained `index.html` — no build step. Open the file directly, or serve it:

```bash
python3 -m http.server 4321
# then open http://localhost:4321
```

## Deploy

Static. Drop the folder on Vercel (or any static host) and it just works — no config needed.

## Notes

- Pointer-events power both mouse drag and touch; tapping an element also drops it in,
  so two taps combine a pair (mobile-friendly).
- The discovery log persists in `localStorage`.
- No audio, no signup, no tracking.
