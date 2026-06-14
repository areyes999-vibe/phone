# 🎵 Chord Encyclopedia

A fully offline chord reference for **ukulele** and **standard-tuning guitar**, built as a
single self-contained web app. Designed for iPhone (e.g. iPhone 12 Pro) but works in any browser.

## What it does
- Pick a **root note** (C, D, F#…) and a **quality** (major), then morph it: tap **minor**, **7**,
  **maj7**, **m7**, **sus4**, **dim7**, **add9**, **9**… to instantly change the chord.
- Shows multiple **voicings** for every chord — each card is the same chord played in a different
  position/voice on the neck, with the fret position labelled (e.g. `5fr`).
- Real **chord-box diagrams**: dots show where to press, ○ = open string, ✕ = muted string,
  the orange dot marks the **root**.
- Toggle the dots between **finger numbers** and **note names**, and read each string's note
  under every diagram.
- Switch between **Ukulele (GCEA)** and **Guitar (EADGB E)** tunings.

Voicings are generated algorithmically from chord formulas + the tuning and ranked for
playability — so every root × quality combination works, not just a hard-coded list.

## Run it offline (no install, no build)
- Just open `index.html` in a browser. That's it — there are no dependencies and nothing loads
  from the network.
- On iPhone: open the page in Safari, tap **Share → Add to Home Screen**. It then launches
  full-screen like a native app and keeps working with no connection.

## Files
- `index.html` — the entire app (UI + chord engine).
- `sw.js`, `manifest.json` — optional PWA support for reliable offline use when served over HTTPS
  (e.g. GitHub Pages).
