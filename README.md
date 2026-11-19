# ScanX Wrapper

A lightweight installable web-app wrapper for ScanX. It embeds the configured Google Apps Script web app in an iframe and includes a fallback direct-open link.

## Files

- `index.html` — entry page and existing Apps Script URL.
- `manifest.webmanifest` — PWA metadata.
- `icon-180.png`, `icon-192.png`, `icon-512.png` — app icons.
- `.nojekyll` — disables Jekyll processing on GitHub Pages.

## Publish with GitHub Pages

1. Create a GitHub repository named `scanx-wrapper`.
2. Upload **the contents** of this folder to the repository root (not a nested folder).
3. In repository **Settings → Pages**, select **Deploy from a branch**, branch **main**, folder **/(root)**, and save.
4. The site URL will be `https://YOUR_USERNAME.github.io/scanx-wrapper/`.

## Notes

- This wrapper relies on an external Google Apps Script Web App; it does not contain the original app's source code.
- The Google Apps Script deployment must permit access for your intended users. Google and browser iframe restrictions can prevent embedded loading; the page includes a direct-open fallback.
- To change the app URL, edit the `APP_URL` variable in `index.html`.
