# Handoff — Blackjack Copilot Landing Site

## What was built

A two-page static GitHub Pages site for the Blackjack Copilot iOS app App Store submission.

| File | Purpose |
|------|---------|
| `index.html` | Marketing landing page |
| `privacy.html` | Privacy policy (required by Apple) |
| `assets/icon.png` | App icon 1024×1024 |
| `assets/ss1–ss4.png` | Four iPhone screenshots |

## App Store URLs

| App Store Connect field | URL |
|-------------------------|-----|
| Marketing URL | `https://blackjackcopilot.github.io` |
| Privacy Policy URL | `https://blackjackcopilot.github.io/privacy` |
| Support URL | `https://github.com/PiotrSkotnicki` |

## Deploy

Push to `main` — GitHub Pages deploys automatically. No build step.

```bash
git add .
git commit -m "Add landing page and privacy policy"
git push
```

## Preview locally

```bash
python3 -m http.server 8080
# open http://localhost:8080
```

## When the App Store link goes live

1. Get the App Store product URL (format: `https://apps.apple.com/app/idXXXXXXXXX`)
2. Replace the "Coming Soon" badge in `index.html` with the real App Store badge and link:

```html
<!-- Replace the .badge-wrap div with: -->
<a href="https://apps.apple.com/app/idXXXXXXXXX" target="_blank" rel="noopener">
  <img src="https://developer.apple.com/assets/elements/badges/download-on-the-app-store.svg"
       alt="Download on the App Store" height="48">
</a>
```

## Asset sources

Originals live in the Blackjack Copilot Xcode project:
- Icon: `BlackjackCopilot/Assets.xcassets/AppIcon.appiconset/icon_1024x1024.png`
- Screenshots: `Screenshots/IMG_3807–3811.PNG`
