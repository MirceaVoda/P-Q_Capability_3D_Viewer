# P-Q Capability 3D Viewer

Static, self-contained viewer for the plant's P-Q / U-Q / P-Q-V capability envelopes
(SC-21 green U-Q/Pmax envelope + SC-18 blue P-Q-V volume, from OLTC-regulated PyPSA
load flow). All capability numbers come from the simulation; the browser only reads them.

## Contents
- `index.html` — the viewer (all CSS/JS inline, no build step, no external assets).
- `commissioning_pq_data.json` — bundled dataset, auto-loaded when the page opens.
  Replace this file to publish a different plant's numbers, or use the in-page
  file-load button to inspect any `commissioning_pq_data.json` locally.

## Deploy (Vercel)
Pure static site — no build. In the Vercel project settings use:
- Framework Preset: **Other**
- Build Command: *(empty / override off)*
- Output Directory: `.`
