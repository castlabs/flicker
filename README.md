# flicker

Minimal image quality flicker tool: flip between original and compressed images, tune interval, and quickly spot subtle artifacts via blink comparison.

## Demo

[![Animated flicker demo comparing the original bunny with a heavily JPEG-quantized version](./flicker-demo.gif)](https://castlabs.github.io/flicker/)

[Open the live demo](https://castlabs.github.io/flicker/)

## Features

- Alternates between two images (`A` and `B`)
- Adjustable flip interval (`200ms` to `5000ms`)
- Zoom with the +/− buttons in steps: 1/8×, 1/4×, 1/2×, 1×, 2×, 4×, 8× (1× is actual image size)
- Drag to pan; zoom and pan stay in place while images alternate
- Semi-transparent zoom panel; drag it to reposition it
- Page scrolling works normally over the image
- Per-image source selection:
  - local upload
  - URL
  - fallback to defaults (`stem-org.jpg`, `stem-os.jpg`)
- Fullscreen support:
  - `Go fullscreen` button
  - image double-click
  - zoom and pan controls remain available in fullscreen

## Run locally

Open `index.html` in a browser.

For local HTTP serving (optional):

```bash
cd git
python3 -m http.server 8000
```

Then open `http://localhost:8000`.
