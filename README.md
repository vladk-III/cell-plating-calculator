# Cell Plating Calculator

A single-page calculator for cell plating. Enter the number of cells you isolated and it returns:

- how many wells you can seed at the target cells per well,
- the M-CSF medium to prepare (with an adjustable pipetting overage),
- the medium and M-CSF stock volumes that reach the final M-CSF concentration.

Defaults: 0.7 × 10⁶ cells per well in 900 µL of suspension, plus 100 µL transfection mix (1 mL final), M-CSF stock 100 µg/mL, final 25 ng/mL, 10% overage. Every value is editable on the page.

## Publish on GitHub Pages

1. Create a new repository on GitHub (for example `cell-plating-calculator`). Public is simplest; private repos need a paid plan for Pages.
2. Upload `index.html` and this `README.md` to the root of the repository (Add file, then Upload files, then Commit).
3. Open the repository's Settings, then Pages.
4. Under "Build and deployment", set Source to "Deploy from a branch", choose the `main` branch and the `/ (root)` folder, and click Save.
5. After about a minute the site is live at `https://<your-username>.github.io/<repository-name>/`.

To change anything later, edit `index.html` in the repository and commit. Pages redeploys on its own.

Notes:
- Fonts load from Google Fonts. Offline, the page falls back to your system fonts and still works.
- The page runs entirely in your browser. Nothing you enter is sent anywhere or saved.
