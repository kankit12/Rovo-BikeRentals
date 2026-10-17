# RoVo

A responsive, Apple-inspired marketing website for RoVo. Built with plain HTML, CSS, JavaScript, and a custom SVG bike illustration. No build step, package manager, external font, CDN, or framework is required.

## Publish on GitHub Pages

1. Unzip this folder.
2. Create a GitHub repository (or use your existing website repository).
3. Upload **the contents of this folder** to the repository root. `index.html` should be at the top level, not inside an additional `rovo` folder. Include the `assets` folder.
4. In the repository, open **Settings → Pages**.
5. Under **Build and deployment**, select **Deploy from a branch**, then your `main` branch and **/ (root)**. Save.
6. GitHub will display your website URL once it finishes publishing. Project URLs work too: all internal links use relative paths.

No API keys or server configuration are needed. The hidden `.nojekyll` file disables unnecessary Jekyll processing; include it if uploading with Git.

## Founder photos and profiles

The four supplied real photos are now embedded directly into `config.js`, in the confirmed order: Ankit, Dillon, Karan, Ved. The file includes photo framing for Ved's full-length photo. No separate photo files or photo folders are needed.

### Updating your existing GitHub website

1. Unzip this download.
2. In your GitHub repository, click **Add file → Upload files**.
3. Upload the new `config.js` to the repository root, alongside `index.html`. Commit changes to replace the old file.
4. Wait for GitHub Pages to rebuild, then refresh the founders page. On Mac, use Command + Shift + R.

Only `config.js` needs replacing to add the photos. The entire source is also included if starting fresh. The separate `assets` folder still contains the bike SVG and favicon and should stay where the original HTML expects it.

Edit names and one-sentence bios near the start of `config.js`. Leave the long embedded image strings intact. Dillon, Karan, and Ved's full names can be added when available. The biographies are editable introductory copy rather than verified job descriptions.

## Files

- `index.html`: home page, concept walkthrough, FAQs.
- `founders.html`: dedicated founders page.
- `styles.css`: all responsive styling, animations, and reduced-motion rules.
- `app.js`: scroll effects, accessible experience tabs, founder rendering.
- `config.js`: editable founder profiles and four embedded real photos.
- `assets/rovo-bike.svg`: original editable bike illustration.
- `assets/icon.svg`: browser favicon.
- `.nojekyll`: GitHub Pages static-site setting.

## Preview locally

Double-click `index.html`, or run from this folder:

```sh
python3 -m http.server 8080
```

Then open `http://localhost:8080`. No installation is needed if Python is already available. The site also works directly from the filesystem.

## Design and behavior

Responsive layouts adapt from small iPhones through desktop monitors. Effects include scroll reveals, desktop bike parallax, a moving text strip, an animated route, hover transitions, and a scroll-progress indicator. System reduced-motion preferences disable motion. The concept walkthrough supports touch, click, arrow keys, Home, and End. FAQs use native accessible disclosure elements.

## Content before launch

This is a marketing website for a developing venture. The map is schematic and clearly labeled as a concept. No claims are made about approved university operations, live bikes, prices, or availability. There is no rental checkout, email collection, app download, or backend hidden behind the buttons. All calls to action lead to actual content on these pages.

Update the development status, FAQs, operational details, founder bios, and brand artwork before announcing an actual service. Photos and the official logo can be added without changing the site architecture.
