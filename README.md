# 3D Oscilloscope Viewer (Single‑File)
Upload your own audio and visualize it in 2D/3D (waveform, spectrum bars, Lissajous, spiral). Record the canvas to a WebM video.

## Live demo (GitHub Pages)
1. Create a **new GitHub repository** (public), e.g. `oscilloscope-3d`.
2. Upload the files from this repo bundle.
3. In the repo settings → **Pages**, set Source to **Deploy from a branch**, select `main` and `/ (root)`.
4. Visit the Pages URL GitHub gives you (usually `https://<user>.github.io/oscilloscope-3d/`).

> The app uses Three.js from **unpkg** CDN, so it works on GitHub Pages out of the box.

## Run locally
- Just open `index.html` in Chrome/Edge/Firefox.
- If modules don’t load on double‑click, start a tiny local server:
  ```bash
  python -m http.server 8000
  # then open http://localhost:8000/index.html
  ```

## Features
- Audio file input (MP3/WAV/etc)
- Modes: Waveform (2D), Spectrum (3D bars), Lissajous (2D), Spiral (3D line)
- Controls: FFT size, smoothing, gain, line width, color
- Orbit camera controls with mouse/touch
- Video capture: exports **WebM (VP9)** of the canvas

> Note: The video capture records the **visual**; it does not include audio. If you want audio muxed too, open an issue and we’ll add it.

## Browser support
- Chrome/Edge/Brave (best), Firefox (good). Safari has partial `MediaRecorder` support.

## License
MIT — see `LICENSE`.
