# ADZUMEX Ads Studio

A free, browser-based advertising platform simulator for practising campaign setup and reading generated campaign metrics. This is an independent simulation and is not affiliated with Google or Meta.

## Demo accounts

- Local demo admin: `admin@adzumex.demo` / `Admin123!`
- Local demo student: `student@adzumex.demo` / `Student123!`
- Each new student starts with ₹100,000 virtual demo credits by default.

These credentials are public demo credentials, not secure accounts. Do not use real passwords or personal information.

## Features

- Google Ads-style campaign practice: Search, Display, Video, Shopping and App.
- Meta Ads-style campaign practice: objectives, audiences, placements and creative selection.
- Campaign launch, pause, resume, manually advance simulation, stop by exhausting budget, and delete.
- Local virtual wallet with reserved, spent, released and allocated credit transactions.
- Local admin demo: create student accounts, allocate credits and reset student demo data.
- Analytics, metric summaries and CSV campaign export.
- Creative library for JPG, PNG, WEBP and MP4 files using browser IndexedDB.
- JSON export/import for local application data. Media blobs are not included in JSON backups.
- Responsive layout for desktop and mobile.

## Run locally

No build step or package installation is required. Open `index.html` in a browser, or serve this folder with any static file server. For example, with Node installed:

```bash
npx serve .
```

## Publish with GitHub Pages

1. Create a GitHub repository named `adzumex-ads-studio-ho` (or use your chosen repository name).
2. Upload all project files and folders from this ZIP to the repository root. Do not upload the ZIP itself as the only file.
3. Open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select branch `main` and folder `/ (root)`, then Save.
6. Wait for deployment. The site should be available at `https://YOUR-USERNAME.github.io/REPOSITORY-NAME/`.

This is a static site. It has no server, backend, database service, secure authentication, or cross-device synchronization. All account, campaign and wallet data stays in the current browser's localStorage. Uploaded creative files stay in that browser's IndexedDB. Clearing site data can delete them. Browser storage can be edited by the user and is not tamper-proof.

## Simulation and wallet rules

- Demo credits are fictional, non-transferable and have no cash value.
- Campaign launch reserves its full total budget from the available balance.
- Each manual simulation run records spend up to the daily budget and remaining reservation.
- Deleting a campaign releases only its unused reserved amount. Historical spend is not refunded.
- Completed campaigns have exhausted their reserved budget.
- Results are generated estimates for practice, not actual or predictive ad performance.

## Important

The app does not connect to Google Ads, Meta Ads, Facebook, Instagram, payment systems or advertising APIs. It does not publish advertisements or charge money. The product names are used only to describe the platforms being simulated.
