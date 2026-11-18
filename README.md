# FramePop Releases

Landing page and release downloads for FramePop, a desktop app that turns UI screenshots into presentation videos. Everything renders locally on your computer: no upload, no account.

Live site: https://tanzir71.github.io/framepop-releases/

## Download

Installers are published on the [Releases page](https://github.com/tanzir71/framepop-releases/releases/latest):

| Platform | Requirement | Asset |
|---|---|---|
| macOS | macOS 14 or newer, Apple Silicon | `FramePop-macOS.zip` |
| Windows | Windows 10 22H2 or newer, x64 | `FramePop-Windows-x64-Setup.exe` (v0.1.0 until the 0.2 Windows build ships) |

FramePop is free during beta. The Windows beta installer is not code-signed yet, so SmartScreen may ask you to confirm before installing. A SHA-256 checksum is published with every release; compare it against your download before running it.

## What FramePop does

- Drop in desktop or mobile screenshots (PNG, JPG, WebP, AVIF). Nothing is cropped, and full-page captures scroll.
- Pick a look (Glide Sequence, Window Stack, Browser Tour, Gallery Zoom, Conveyor, Responsive Pair and more). It plays your whole set, with a transition at every boundary.
- Reorder in the storyboard or the Arrange grid. Transitions re-link and the preview follows.
- Add camera moves, emphasis (zoom to region, spotlight, callouts, cursor) and text (titles, lower thirds, captions, end cards).
- Subtle studio backdrops, your own colour, image or video, and an optional desktop menu bar and dock.
- Export presets for landing pages, Product Hunt, X, LinkedIn, Reels, App Store previews, YouTube 4K, Keynote and docs.
- Formats: MP4, HEVC, ProRes 4444 with alpha, ProRes 422 HQ, WebM, GIF and PNG sequences, with real motion blur, up to 4K 60fps.

## About this repository

This repo contains only the static marketing site, served with GitHub Pages, and hosts the release downloads. The application source is not in this repository.

- `index.html`: the single-page site
- `media/v2/`: the hero, look loops, posters and backdrop stills (all rendered by FramePop itself)
- `_astro/`: compiled stylesheet and script
- `brand/`, `favicon.svg`, `favicon-32.png`, `apple-touch-icon.png`, `og-image.png`: brand mark, icons and share image
- `site.webmanifest`, `robots.txt`, `.nojekyll`: site metadata and Pages config

To preview the site locally, serve the folder with any static file server, for example `python3 -m http.server` from the repo root, then open `http://localhost:8000`.
