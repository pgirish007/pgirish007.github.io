Drop screenshots here with these exact filenames and the landing page (`../index.html`) will pick them up automatically once you swap the placeholder `<div class="shot-placeholder">` blocks for `<img>` tags (see the HTML comment right above each one):

| Filename | Used for | Suggested shot |
|---|---|---|
| `hero.png` | Top hero image | The dialog's "Watermark style" section, or a nice finished watermarked astrophoto |
| `source.png` | Gallery 1 | The "Target image" view picker |
| `reference.png` | Gallery 2 | The "Reference metadata source" section — open view or FITS/XISF file browser |
| `dialog.png` | Gallery 3 | Full dialog showing target/reference/fields + the style controls |
| `preview.png` | Gallery 4 | The live preview panel mid-drag, or with the 3x3 position grid visible |
| `result.png` | Gallery 5 | A before/after or just the final image with the watermark baked in |

All five gallery images open in a click-to-enlarge lightbox (with a ✕ close button) automatically — no extra work needed once you swap in the `<img ... onclick="openLightbox(this)">` tag shown in the HTML comment above each placeholder.

Tips:
- PNG, ~1200-1600px wide is plenty — this page displays them scaled down.
- On macOS, `Cmd+Shift+4` then `Space` captures a single window (the PixInsight dialog) cleanly.
- Crop out anything you don't want visible (file paths, other open images, etc.) before saving.
