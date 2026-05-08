# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a single-file web app: a two-player Tic Tac Toe game playable in any browser.

- **Entry point:** `index.html` — contains all HTML, CSS, and JavaScript inline.
- No build step, no dependencies, no server required. Open `index.html` directly in a browser.

## Architecture

Everything lives in `index.html`:

- **HTML** — 9 `.cell` divs with `data-i` attributes (0–8) form the board.
- **CSS** — Dark theme using CSS Grid for the board layout.
- **JS** — Vanilla JS. State is `board[]` (9-element array), `current` (X/O), `gameOver`, and `scores`. Win detection checks all 8 winning lines in `WINS`. Event delegation on `#board` handles all cell clicks.

## Running

```bash
open index.html
```
