# Audio Editing Comparisons (anonymous review package)

Static comparison page for the paper **Null-Space Alignment for Inversion-Free Music Editing**.
The page shows the original/edit prompts, the source audio, and the outputs of nine methods
(Ours, MusicMagus, ZETA, SteerMusic, FireFlow, RF-solver, DirectAudioEdit, FLowEdit,
Ablation alpha=0.3).

## Contents
- `index.html` — comparison page (one big title, two sections: MelodiaEdit and ZoME-Bench)
- `data_v3.json` — sample list and method/audio mapping (embedded into `index.html` at build time)
- `audio/` — 310 mp3 clips (original + 9 methods per sample)
- `figures/coefficient_schedules.png` — orthogonal-coefficient schedules (NSA vs FlowDC)

## Run locally
Serve the folder over HTTP:

```bash
python3 -m http.server 8000
# open http://localhost:8000/
```

## Note
The comparison page is self-contained: sample data is embedded in `index.html`, and all audio
is referenced with relative paths, so the page can be rendered from a static host or from an
anonymous review service without any server-side code.
