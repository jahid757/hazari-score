# Hazari Score Keeper: Landing Page

A simple, professional, single-file landing page for **Hazari Score Keeper**, an offline scorekeeper app for the card game Hazari.

## Overview

The page presents the app's features, screenshots, and download link in a clean green-and-gold design that matches the app's UI. It is built with plain HTML and CSS only, with no frameworks, no build step, and no JavaScript.

## Features

- Responsive layout (desktop, tablet, mobile)
- Sticky navigation bar
- Hero section with a CSS-built phone mockup
- Feature grid, app screenshots, "How it works" steps, and a download call-to-action
- No image files required, since the screenshots are drawn with CSS
- Single file, easy to host anywhere

## Project Structure

```
.
├── index.html   # The complete landing page (HTML + CSS)
└── README.md
```

## Getting Started

1. Download or copy `index.html` into a folder.
2. Open it in any modern browser (double-click the file).

No installation or server is needed.

## Customization

### Download link
Find the download buttons and replace `href="#"` with your APK or Play Store link:

```html
<a href="https://github.com/jahid757/hazari-score/blob/main/app/Hazari%20Score%20Keeper.apk" class="btn btn-gold">⬇ Download for Android</a>
```

The nav "Download" button points to `#download`, which scrolls to the bottom call-to-action section.

### Colors
Theme colors are defined as CSS variables at the top of the `<style>` block:

```css
:root{
  --green-900:#0b3d2b;
  --green-800:#0f4a34;
  --green-700:#145c40;
  --gold:#d4a62a;
  --gold-light:#f0c84b;
}
```

### Real screenshots
To use actual app screenshots instead of the CSS mockups, replace the contents of a `.screen` element with an image:

```html
<div class="phone sm">
  <div class="screen">
    <img src="screenshots/home.png" alt="Home screen" style="width:100%;height:100%;object-fit:cover">
  </div>
</div>
```

### Text and footer
Edit the headings, feature descriptions, version number, and author name directly in `index.html`.

## Deployment

Because the site is a single static file, it can be hosted for free on:

- **GitHub Pages**: push the folder to a repo, then enable Pages in the repo settings
- **Netlify**: drag and drop the folder at app.netlify.com/drop
- **Vercel** or **Cloudflare Pages**: connect the repo or upload the folder

## Browser Support

Works on all modern browsers (Chrome, Edge, Firefox, Safari). It uses CSS Grid, Flexbox, and CSS variables.

## Fonts

The page uses the [Inter](https://fonts.google.com/specimen/Inter) font from Google Fonts. If the user is offline, it falls back to the system font automatically.

## About the App

Hazari Score Keeper is a simple offline scorekeeper for the card game Hazari. All data stays on your device and nothing is ever uploaded.

- Version: 2.0
- Built by Jahid

