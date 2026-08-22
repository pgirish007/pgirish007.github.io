Images used by the landing page (`../index.html`). All wired in with `<img ... onclick="openLightbox(this)">`, so every one opens in the click-to-enlarge lightbox already.

| Filename | Used for | Content |
|---|---|---|
| `hero.jpg` | Top hero image + gallery 5 (result) | Finished watermarked astrophoto |
| `source.jpg` | Gallery 1 | The target astrophoto before watermarking |
| `reference.jpg` | Gallery 2 | Raw sub-frame whose FITS header supplies the watermark text |
| `dialog.png` | Gallery 3 | The empty dialog — fields + style controls |
| `preview.png` | Gallery 4 | The dialog with a view loaded and the live preview rendered |

Notes:
- `hero.jpg`, `source.jpg` and `reference.jpg` are photographic (noisy astro images), so they're saved as JPEG — much smaller than PNG for this kind of content with no visible quality loss. `dialog.png` and `preview.png` are UI screenshots (flat colors, text) where PNG is the right call — keep those as PNG if you replace them.
- To replace any image, keep the same filename and just overwrite the file — no HTML changes needed.
- To add a genuinely new slot, copy an existing `<figure>` block in `index.html`'s `#screenshots` gallery, point its `src` at your new file, and it'll pick up the lightbox/hover behavior automatically.
