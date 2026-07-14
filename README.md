# tsukami-texthooker (掴み)

A minimal, single-file texthooker for reading Japanese text (manga, VNs, games) captured via a clipboard-watching OCR/hook tool.

## Setup

1. Download `texthooker.html` (or clone this repo).
2. Open it in a Chromium-based browser (Chrome or Edge) — double-click the file, or drag it into a tab.
3. Install a clipboard-watching extension, e.g. **Clipboard Inserter Redux**, and enable it for this page. It should append clipboard text as a bare `<p>` tag to the page — that's what this page watches for.
4. Point your text-hook / OCR tool (Textractor, manga-ocr, etc.) so its output goes to your OS clipboard.
5. Read — every new clipboard entry appears as a new line automatically.

## Features

- 🗑️ Clear all lines
- 🕒 Toggle timestamps
- A-/A+ Adjust font size
- 🌓 Light/dark theme
- 📖 Focus mode — hides the toolbar and footer for distraction-free reading (press `Esc`, or click the faint ✕ in the top-right corner, to exit)
- ⛶ Browser fullscreen
- 🪟 Floating window — pops the log out into an always-on-top window (Chrome/Edge 116+, via the Document Picture-in-Picture API) that stays visible even over other full-screen apps
- Manual line entry (type into the box + Enter) for notes
- Auto-scroll, with a "↓ new lines" button when you've scrolled up and don't want to jump

## Notes

- All data — captured lines and your preferences — is stored in your browser's `localStorage`, scoped to wherever you opened the file from. Nothing is sent anywhere.
- Floating window mode requires a Chromium-based browser that supports the Document Picture-in-Picture API.
