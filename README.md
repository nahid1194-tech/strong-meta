# Strong Meta + Map Section

Static website bundle prepared for GitHub and GitHub Pages.

## Included
- `index.html` — Strong Meta interface with the **Map Section** navigation item.
- `map/index.html` and `map/assets/` — bundled Vector Map Generator app.
- `.nojekyll` — tells GitHub Pages to publish files without Jekyll processing.

## Upload to GitHub
1. Create a repository on GitHub.
2. Upload the contents of this folder to the repository root (not the ZIP file itself).
3. Confirm that `index.html`, `.nojekyll`, `README.md`, and the `map/` folder appear at the top level.
4. Open **Settings → Pages**.
5. Under **Build and deployment**, select **Deploy from a branch**.
6. Choose branch `main` and folder `/(root)`, then click **Save**.
7. Wait for deployment and open the URL shown in the Pages section.

## Important notes
- Keep `index.html` beside the `map/` folder; the Map Section iframe uses the relative path `map/index.html`.
- The map app retrieves some geographic data from public external CDN/GitHub URLs, so those requests require an internet connection and the external data providers to remain available.
- This package is static-only. Any API key or browser-side AI feature should be configured carefully; never commit private API keys to a public repository.
- The app's JavaScript syntax was checked, but a full live GitHub Pages browser test has not been performed.
