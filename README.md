# WhatItFeelsLike — Website

A self-contained presentation site for the **WhatItFeelsLike** project — a research prototype that takes everyday video of an environment, surfaces sensory triggers, and renders a sensory-modulated version of the same clip to support informed decisions about autism-friendly spaces.

> Augmented Human Lab · Labothon · Team 02
> Ariel · Bell · Maria · Sankha · Soundarya

## Browse

- `index.html` — the site itself (About + Results tabs)
- `uploads/` — original input clips
- `results/<job_id>/` — per-clip processed video (`*_final.mp4`) and structured report (`*_report.json`)
- `assets/` — AHL brand mark

## Local preview

Open `index.html` directly in a browser, or:

```bash
python -m http.server 8000
# then visit http://localhost:8000
```

Some browsers block inline `<video>` autoplay/preload from `file://` URLs; the `python -m http.server` route is the most reliable for offline review.

## Source

This site is a static export from the working repo at
[`augmented-human-lab/wiflike-fast`](https://github.com/augmented-human-lab/wiflike-fast)
(or the team's local checkout). Regenerate with:

```bash
python scripts/build_static.py --output dist
```
