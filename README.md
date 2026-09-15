# TripSplit Pro

A mobile-first, installable trip expense splitter for GitHub Pages. No build step is required.

## Features
- Multiple trips and travellers
- Natural-language expense prefilling
- Equal or selected-member splits
- Optimized net settlements
- Multiple currencies and settlement currency choice
- Historical exchange-rate lookup via Frankfurter with Google/manual fallback
- Categories and receipt photos
- Edit/delete expenses
- Offline PWA support
- JSON export/import backup
- Native share sheet
- Apple-inspired dark interface

## Publish on GitHub Pages
1. Create an empty GitHub repository.
2. Upload every file in this package to the repository root. Do not upload the containing folder.
3. In the repository, open **Settings > Pages**.
4. Under **Build and deployment**, select **Deploy from a branch**.
5. Select **main** and **/(root)**, then save.

## Local preview
Because service workers require HTTP, run a local server instead of double-clicking index.html:

```bash
python3 -m http.server 8080
```

Then open `http://localhost:8080`.

## Notes
- Data is stored locally in the browser. Use Export JSON backup before clearing browser data or moving devices.
- The automatic rate source may not support every currency. In that case, use Google Verify and save the rate manually.
- Receipt images are compressed only by the browser/device and can increase local-storage usage.
