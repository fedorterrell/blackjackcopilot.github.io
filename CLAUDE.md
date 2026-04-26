# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project

Landing site for the Blackjack Copilot app, hosted on GitHub Pages at `blackjackcopilot.github.io`. The remote is `https://github.com/fedorterrell/blackjackcopilot.github.io.git`.

## Deployment

This is a GitHub Pages site — pushing to `main` deploys automatically. There is no build step; serve files directly from the repo root. To preview locally:

```bash
python3 -m http.server 8080
```

## Git LFS

The repo has Git LFS configured (`git lfs` must be installed). Any large binary assets (images, fonts, videos) should be tracked with LFS rather than committed as raw blobs.
