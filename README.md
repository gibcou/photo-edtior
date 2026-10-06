# Photo Editor

A self-contained, browser-based video and photo editing tool ("Cutting Room"), built as a single HTML file — no install, no backend, runs entirely client-side.

## Features

- Timeline-based video/photo editing with clip trimming, reordering, and transitions (cross-fade, slide)
- Built-in color looks plus manual color grading (exposure, contrast, highlights, shadows, whites, blacks, temperature, tint, saturation)
- Custom preset import: load your own `.cube` 3D LUT files or Lightroom `.xmp` develop presets and apply them to any clip
- Auto-fix: automatic exposure, white balance, and highlight/glare correction applied to newly added photos and videos
- Video stabilization: reduces camera shake/jitter in shaky footage
- Text captions, background music with beat-sync snapping, auto-editing presets
- Multiple aspect ratios (9:16, 1:1, 16:9) for exporting to different platforms

## Usage

Open `index.html` in a modern desktop browser (Chrome, Edge, or Firefox recommended). All processing happens locally in the browser; no files are uploaded to any server.

## Importing presets

Select a clip, then use the "Import preset (.cube / .xmp)" button in the inspector panel to load a LUT or Lightroom preset file. `.cube` LUTs are applied exactly as authored. `.xmp` Lightroom presets are approximated from their basic develop sliders (exposure, contrast, tone, color, temperature/tint) — split toning, parametric tone curves, and local/masked adjustments from Lightroom are not reproduced, since those aren't representable outside Lightroom's own engine.
