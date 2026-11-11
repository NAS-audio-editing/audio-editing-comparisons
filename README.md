# Audio Editing Comparisons (anonymous review package)

Static comparison page for the paper **Null-Space Alignment for Inversion-Free Music Editing**.
The page shows the original/edit prompts, the source audio, and the outputs of nine methods
(Ours, MusicMagus, ZETA, SteerMusic, FireFlow, RF-solver, DirectAudioEdit, FLowEdit,
Ablation alpha=0.3). Sample identifiers and CLAP scores are intentionally hidden.

## Contents
- `index.html` — comparison page (one big title, two sections: MelodiaEdit and ZoME-Bench)
- `data_v3.json` — sample list and method/audio mapping
- `audio/` — 310 mp3 clips (original + 9 methods per sample)
- `figures/coefficient_schedules.png` — orthogonal-coefficient schedules (NSA vs FlowDC)
- `null-space-alignment-for-inversion-free-music-editing/` — convenience path (redirect)

## Run locally
The page uses `fetch()`, so serve it over HTTP (not `file://`):

```bash
cd null-space-alignment-site   # or the repository root
python3 -m http.server 8000
# open http://localhost:8000/
```

## Data
Full data archive (same content as this package): **<FIGSHARE_PRIVATE_LINK>**

## Anonymous repository
**<ANONYMOUS_GITHUB_LINK>**
