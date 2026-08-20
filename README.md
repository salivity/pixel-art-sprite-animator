# Pixel Art Sprite Animator

An in-browser tool for slicing, testing, chroma-keying, and exporting 2D sprite sheets into animated sequences. Built with vanilla JavaScript, HTML5 Canvas, and Tailwind CSS.

**Live Demo:** [https://salivity.github.io/pixel-art-sprite-animator](https://salivity.github.io/pixel-art-sprite-animator)

---

## Features

* **Flexible Grid Slicing:** Supports square sheets from **1×1 up to 5×5** (1 to 25 frames) with real-time grid mapping and frame re-indexing.
* **Chroma Key Removal:** Live color-picker and adjustable tolerance slider to strip background colors (such as green-screen or magenta backgrounds) with transparency.
* **Stage & Playback Controls:**
  * Variable framerate control (1–60 FPS).
  * Frame stepping and play/pause controls.
  * Directional flipping (Left/Right mirroring).
  * Horizontal stage traversal mode.
  * Canvas zoom controls (25% to 500%) with pixelated rendering preservation.
* **Export Options:**
  * **Animated PNG (APNG):** High-color lossless animated PNG output.
  * **Transparent GIF:** Multi-threaded client-side GIF rendering with transparency preservation.
  * **CSS Keyframe Generator:** Ready-to-use CSS keyframe snippets for web game projects.
* **State Persistence:** Preserves frame counts, padding, speeds, and dark/light mode preferences in `localStorage`.
* **Zero Server Dependencies:** Fully client-side processing using Web Workers and HTML Canvas.

---

## Tech Stack & Libraries

| Category | Technology |
|---|---|
| **UI & Styling** | Tailwind CSS (CDN), FontAwesome 6, Google Fonts (*Inter*, *Fira Code*) |
| **Rendering Engine** | HTML5 Canvas 2D API |
| **APNG Generation** | [UPNG.js](https://github.com/photopea/UPNG.js) & [pako](https://github.com/nodeca/pako) |
| **GIF Generation** | [gif.js](https://github.com/jnordberg/gif.js) |

---

## Quick Start

### 1. Run Locally
No build step or Node.js environment is required. Clone the repository and open `index.html` in any modern browser:

```bash
git clone [https://github.com/salivity/pixel-art-sprite-animator.git](https://github.com/salivity/pixel-art-sprite-animator.git)
cd pixel-art-sprite-animator
