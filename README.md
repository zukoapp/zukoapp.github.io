# Zuko — GitHub Pages site

Static site that hosts the Zuko privacy policy, terms, and support page. Required by App Store Connect (privacy URL is mandatory) and linked from inside the app.

## Deployed

Hosted as GitHub Pages **user site** at `appzuko/zukoapp.github.io` (root).

Live URLs:
- `https://zukoapp.github.io/`
- `https://zukoapp.github.io/privacy.html`
- `https://zukoapp.github.io/terms.html`
- `https://zukoapp.github.io/support.html`

Push to `main` to deploy. `AppURLs.base` in `Zuko/Services/DiagnosticsInfo.swift` is the single source of truth — change it if you move to a custom domain.

## Custom domain later

If you register a real domain (e.g. zuko.app), add a `CNAME` file to this folder with the domain, configure DNS, and update `AppURLs.base`.
