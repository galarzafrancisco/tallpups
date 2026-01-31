# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Tall Pups is a minimal static landing page. Currently consists of a single `index.html` file with inline CSS - no build system or dependencies.

## Development

To view the site locally, open `index.html` in a browser or use any static file server:

```bash
npx serve .
# or
python3 -m http.server
```

## Architecture

- **index.html**: Single-page landing with inline styles. Uses serif typography (Georgia), responsive text sizing via `clamp()`, and a centered flexbox layout.
