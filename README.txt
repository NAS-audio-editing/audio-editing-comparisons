Audio Editing Comparisons — portable static site
================================================

Serve over HTTP (the page uses fetch(), so file:// will not work):

    cd null-space-alignment-site
    python3 -m http.server 8000
    # open http://localhost:8000/

Contents
  index.html      comparison page (one big title; no CLAP scores or file names)
  data_v3.json    sample list: MelodiaEdit (24 samples) + ZoME-Bench (7 samples)
  audio/          310 mp3 clips (original + 9 methods per sample)
  figures/        coefficient_schedules.png
  null-space-alignment-for-inversion-free-music-editing/index.html
                  convenience path that redirects to ../index.html

Methods per sample (9): Ours, MusicMagus, ZETA, SteerMusic, FireFlow,
RF-solver, DirectAudioEdit, FLowEdit, Ablation alpha=0.3
