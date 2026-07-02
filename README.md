# Classic arXiv Red

A tiny Manifest V3 Chrome extension that restores arXiv's classic crimson
header. It contains no JavaScript, no analytics, no network requests, and no
general-purpose Chrome permissions.

## Project structure

```text
classic-arxiv-red/
├── manifest.json
├── styles.css
├── icons/
│   ├── icon-16.png
│   ├── icon-32.png
│   ├── icon-48.png
│   └── icon-128.png
├── PRIVACY.md
├── STORE_LISTING.md
└── LICENSE
```

## Run it locally

This plugin is not yet published on the Chrome Web store, but for now can be straightforwardly run locally:
1. Open `chrome://extensions`.
2. Enable Developer mode.
3. Click *Load unpacked*.
4. Select this `classic-arxiv-red` directory.
5. Open or refresh `https://arxiv.org/`.

## Development notes

- The extension statically injects `styles.css` on `arxiv.org`.
- It intentionally requests no `permissions`.
- The current selectors begin with `.ds-site-header`.