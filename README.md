# Cell Plating Calculator

A single-page calculator for cell plating. Enter the number of cells you isolated and it returns:

- how many wells you can seed at the target cells per well,
- the M-CSF medium to prepare (with an adjustable pipetting overage),
- the medium and M-CSF stock volumes that reach the final M-CSF concentration.

Defaults: 0.7 × 10⁶ cells per well in 900 µL of suspension, plus 100 µL transfection mix (1 mL final), M-CSF stock 100 µg/mL, final 25 ng/mL, 10% overage. Every value is editable on the page.

## Publish on GitHub Pages

1. Create a new repository on GitHub (for example `cell-plating-calculator`). Public is simplest; private repos need a paid plan for Pages.
2. Upload every file in this folder (`index.html`, `sw.js`, `manifest.webmanifest`, the four `.png` icons and this `README.md`) to the root of the repository (Add file, then Upload files, then Commit).
3. Open the repository's Settings, then Pages.
4. Under "Build and deployment", set Source to "Deploy from a branch", choose the `main` branch and the `/ (root)` folder, and click Save.
5. After about a minute the site is live at `https://<your-username>.github.io/<repository-name>/`.

To change anything later, edit `index.html` in the repository and commit. Pages redeploys on its own.

Notes:
- Fonts load from Google Fonts. Offline, the page falls back to your system fonts and still works.
- The page runs entirely in your browser. Nothing you enter is sent anywhere or saved.

## Install it as an app (iPhone, iPad, Mac)

The page has an "Install app" button and a "Download file" button under the title. "Install app" installs directly in Chrome and Edge. In Safari it shows the steps below, because Safari does not allow a page to start the install itself. "Download file" saves a single copy of the page (`cell-plating-calculator.html`) that opens in any browser. The buttons disappear once the app is installed.

Open the live site once while online, then:

- **iPhone or iPad (Safari):** tap Share, then "Add to Home Screen", then Add. It opens full screen with its own icon and works offline.
- **Mac (Safari 17 or later):** File, then "Add to Dock". It gets its own app window and Dock icon.
- **Mac (Chrome or Edge):** click the install icon at the right end of the address bar.

On iPhone and iPad this has to be done from Safari. Other iOS browsers do not offer "Add to Home Screen" for every site.

## Updating an installed copy

Installed copies keep a saved version of the site. After you change any file, open `sw.js` and increase the number in `VERSION` (for example `plating-v2`). The next time the app opens online, it picks up the new version. Close and reopen the app once if it still shows the old one.
