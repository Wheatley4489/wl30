# Wheatley WL-30

A two-line scientific calculator for iPad, laid out and operated like the TI-30XIIS that students use in class. It runs in Safari, installs to the Home Screen as a full-screen app, and keeps working offline after the first visit.

## Files

| File | What it is |
|---|---|
| `index.html` | The whole calculator (markup, styles and logic in one file) |
| `manifest.webmanifest` | App name, colors and icons for "Add to Home Screen" |
| `sw.js` | Service worker that caches the app so it works offline |
| `icons/` | Home Screen and browser icons |
| `.nojekyll` | Tells GitHub Pages to serve the files as they are |

## Publish with GitHub Pages

1. Create a new repository on GitHub, for example `wl30-calculator`. It must be public for GitHub Pages on a free account.
2. Upload every file and the `icons` folder to the root of the repository (Add file › Upload files, then commit).
3. Open **Settings › Pages**. Under **Build and deployment**, set **Source** to *Deploy from a branch*, choose `main` and `/ (root)`, and save.
4. After a minute or two the page shows your address, usually `https://YOUR-USERNAME.github.io/wl30-calculator/`.

## Install on an iPad

1. Open the address in **Safari**.
2. Tap the **Share** button, then **Add to Home Screen**, then **Add**.
3. Launch it from the new WL-30 icon. It opens full screen, without the Safari toolbar.

Open it once while online so it can save itself for offline use. Settings, memory variables (A–E) and statistics data are kept on each iPad.

For a class set, share the address with a QR code, or ask your IT team to push it as a web clip through your device management system.

## Updating

Edit `index.html`, then change `VERSION` at the top of `sw.js` (for example `wl30-v2`) and commit both. iPads pick up the new version the next time the app is opened online.
