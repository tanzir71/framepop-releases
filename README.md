# FramePop Releases

Landing page and release downloads for FramePop, a desktop app that turns UI screenshots into presentation videos. Everything renders locally on your computer: no upload, no account.

Live site: https://tanzir71.github.io/framepop-releases/

## Download

Installers are published on the [Releases page](https://github.com/tanzir71/framepop-releases/releases/latest):

| Platform | Requirement | Asset |
|---|---|---|
| macOS | macOS 14 or newer, Apple Silicon | `FramePop-macOS.zip` |
| Windows | Windows 10 22H2 or newer, x64 | `FramePop-Windows-x64-Setup.exe` |

FramePop is free during beta. The Windows beta installer is not code-signed yet, so SmartScreen may ask you to confirm before installing. A SHA-256 checksum is published with every release; compare it against your download before running it.

## What FramePop does

- Drop in PNG, JPG, WebP or AVIF screenshots, pick a motion template, and export a video.
- Content-aware layout sizes each card from your image instead of cropping it to a fixed frame.
- Optional device frames, adjustable shadows, custom backgrounds, and several aspect ratios (16:9, 1:1, 4:5, 9:16).
- Full-page captures scroll to reveal themselves.
- Save your own looks as reusable templates.
- Exports up to 4K at 60 fps, encoded on-device with the native H.264 encoder on macOS and Windows.

## About this repository

This repo contains only the static marketing site, served with GitHub Pages, and hosts the release downloads. The application source is not in this repository.

- `index.html`: the single-page site
- `media/`: template previews and demo videos
- `_astro/`: compiled stylesheets
- `site.webmanifest`, `robots.txt`, `app-icon.svg`, `.nojekyll`: site metadata and Pages config

To preview the site locally, serve the folder with any static file server, for example `python3 -m http.server` from the repo root, then open `http://localhost:8000`.
