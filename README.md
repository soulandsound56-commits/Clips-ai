# FreeClip

Free, browser-based video clipper with auto captions. No server, no uploads, no cost.

## Features
- Clip videos up to **7 hours** long
- **1080p** support (export Original, 1080p, 720p or 480p)
- **Auto captions** (Whisper running in your browser) with live preview, `.srt` and `.vtt` download
- 100% free, hosted on GitHub Pages

## Deploy on GitHub Pages
1. Create a new public repository (e.g. `freeclip`).
2. Upload `index.html` and this `README.md` to the repo root.
3. Go to **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**, select `main` and `/ (root)`, then **Save**.
5. After a minute your site is live at `https://YOUR-USERNAME.github.io/freeclip/`.

## Notes
- Long videos are read lazily from disk (not loaded into RAM), so 7-hour files work for cutting.
- "Original" quality is a fast stream copy (cuts at the nearest keyframe).
- Re-encoding to 1080p/720p/480p and captioning run on the user's device, so use shorter clips for those.
- Needs a modern browser (Chrome, Edge or Firefox recommended). WebGPU makes captions faster when available.
