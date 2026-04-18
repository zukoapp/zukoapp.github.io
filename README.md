# SubWise — GitHub Pages site

Static site that hosts the SubWise privacy policy, terms, and support page. Required by App Store Connect (privacy URL is mandatory) and linked from inside the app.

## Deploy

1. Create a public GitHub repo named `subwise` under the `appsubwise` account (matches the assumed URL in `SubWise/Services/DiagnosticsInfo.swift` → `AppURLs.base`).
2. Push the contents of **this `docs-site/` folder** to the repo root on `main`.
3. In repo Settings → Pages: source = `main` branch, folder = `/ (root)`. Save.
4. Pages builds in ~30s. Verify URLs:
   - `https://appsubwise.github.io/subwise/`
   - `https://appsubwise.github.io/subwise/privacy.html`
   - `https://appsubwise.github.io/subwise/terms.html`
   - `https://appsubwise.github.io/subwise/support.html`

## If your GitHub username is not `appsubwise`

Change `AppURLs.base` in `SubWise/Services/DiagnosticsInfo.swift` to match — that's the single source of truth. Then update `fastlane/metadata/en-US/privacy_url.txt`, `support_url.txt`, `marketing_url.txt`.

## Custom domain later

If you register a real domain (e.g. subwise.app), add a `CNAME` file to this folder with the domain, configure DNS, and update `AppURLs.base`.
