# Assets — drop-in files for the project page

The page is fully self-contained (`../index.html`) and works with placeholders.
Replace these to make it production-ready:

## Figures (Results section)
Copy straight from `paper_assets/figures/performance/`:

| Filename expected here | Source |
|---|---|
| `radar_combined.png` | `paper_assets/figures/performance/radar_combined.png` |
| `qa_forest.png`      | `paper_assets/figures/performance/qa_forest.png` |

If a file is missing, the page shows a labelled placeholder instead of breaking.

## Demo clips (The Stream)
The demo viewport currently renders an abstract, task-tinted placeholder scene.
To use real footage, add per-demo assets here (e.g. `ic-text.mp4` /
`ic-text.webm`, or a sampled frame sequence / GIF) and wire them into the `.vp`
element inside `mountStream()` in `index.html`.

⚠ Ego4D is license-gated — confirm redistribution is permitted before hosting raw
clips publicly. Safer options: sampled frames, short low-res segments if allowed,
or self-recorded first-person clips we own.

## Numbers to replace before publishing
- `RESULTS` array in `index.html` — currently **illustrative**. Swap in the
  values from `paper_assets/tables/qa_accuracy/`.
- Author list, affiliations, BibTeX, and the Paper/Code/Data/Leaderboard links.
