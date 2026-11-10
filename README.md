# Prompter by Fourside Studios

A free teleprompter web app for iPad, built for real shoots.

**Use it:** https://prompter.foursidestudios.com

Open it in Safari on an iPad, tap Share, then **Add to Home Screen**. It runs full screen like an app.

## Features

- Speed set in words per minute, so large text never slows the scroll
- Bluetooth remote and clicker support, with a guided setup that learns any remote's buttons
- Hold Next or Back to change speed on simple two-button clickers
- Mirror and flip for beam-splitter glass rigs
- Adjustable text size, line spacing, margins and reading line, live while prompting
- Paragraph jumps for quick retakes
- Import from `.txt` files or Google Docs
- Scripts are saved on the device only

## Files

| File | Purpose |
| --- | --- |
| `index.html` | The whole app: markup, styles and script |
| `version.json` | Latest version number, read by the in-app update check |
| `privacy.html` | Privacy policy (required for Google sign-in) |
| `manifest.webmanifest` | Home screen install settings |
| `icon.svg`, `*.png` | App icons |
| `CNAME` | Custom domain for GitHub Pages |

## Google Docs import

Fill in `GOOGLE.clientId`, `GOOGLE.apiKey` and `GOOGLE.appId` near the bottom of `index.html`. The OAuth client must list `https://prompter.foursidestudios.com` as an Authorized JavaScript origin.

## Releasing an update

See [RELEASING.md](RELEASING.md).

## Self-hosting

Prompter is a static web app with no build step. Copy every file in this repo to any web server with HTTPS and open `index.html`. To use Google Docs import on your own server, create your own Google Cloud project and fill in the `GOOGLE` values in `index.html`.

## License

Copyright (C) 2026 Fourside Studios LLC.

Prompter is free software released under the [GNU Affero General Public License v3.0](LICENSE). You can use, modify and self-host it. If you run a modified version for other people over a network, you must make your modified source code available to them under the same license.

---

Made by [Fourside Studios](https://www.foursidestudios.com), Palmer, MA.
