# Listen - We Were Here archive

A tiny, self-contained shuffle player for the **We Were Here** digital archive
(*The African American Experience in Boyle County, Kentucky*).

Press **Start listening** and the app shuffles through ~150 narrated photographs
from the archive, playing each as a YouTube clip (the photograph on screen while
a narrator speaks), auto-advancing clip to clip. Each item links back to its
page in the Omeka archive.

## Files

- `index.html` - the whole app: vanilla JS + the YouTube IFrame API, no build
  step and no dependencies. The playlist is embedded directly in the file.
- `manifest.json` - the playlist (`pn`, `videoId`, `title`, `itemUrl`), also
  embedded in `index.html`. Regenerate from `narration_ledger.csv` if the
  archive changes.

## Controls

- **Next ▷** / **Pause**
- Keyboard: `Space` play/pause · `N` or `→` next
- Auto-advances when a clip ends; unplayable clips are skipped quietly.

## Hosting

Served via GitHub Pages from `main` / root, and embedded in the archive's
"Listen" page via an iframe.

*Phase 1: narrated photographs. A later phase may add the oral-history audio clips.*
