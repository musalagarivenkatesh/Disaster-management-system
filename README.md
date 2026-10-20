# Disaster Response Hub — Reconstructed Frontend

This project is a **reconstruction**, not the original source code recovered from Vercel. It is based on the publicly visible pages and content of the deployed academic demo at `https://disaster-response-frontend-iota.vercel.app/`.

## Included pages

- `index.html` — public homepage / overview
- `incidents.html` — searchable incident registry
- `alerts.html` — sample alert feed and safety reminder
- `resources.html` — searchable sample inventory
- `volunteers.html` — searchable roster and local-only demo registration
- `report-incident.html` — local-only incident report form
- `map.html` — schematic map-style view with sample markers and filters
- `analytics.html` — illustrative metrics and charts
- `dashboard.html` — authority dashboard mock-up
- `login.html` — sign-in screen mock-up
- `styles.css` — responsive styling
- `app.js` — page rendering and front-end demo interactions

## Important limitations

- This is a static frontend demo. No backend, API, database, actual authentication, GIS integration, or dispatch connection is included.
- Incidents and volunteers submitted through the forms are stored only in the current browser's `localStorage`; they are not uploaded anywhere.
- Default alerts, counts, incident entries, and locations are sample data. They are not live, verified emergency information.
- Do not use this project to report a real emergency. Contact the appropriate official emergency service directly.
- The public Vercel URL does not expose the original project source reliably. The Vercel source inspector (`/_src`) normally requires access to the owning Vercel account/team. This reconstruction does not reproduce the original backend or guarantee pixel-perfect matching.

## Run locally

No build tools or packages are required. Open `index.html` in a browser. For a local web server, run one of these commands from this folder:

```bash
python -m http.server 8000
```

Then open `http://localhost:8000`.

## Push to GitHub from Windows / VS Code

1. Extract this ZIP to a normal folder.
2. Open that folder in VS Code.
3. Open **Terminal → New Terminal**.
4. Run:

```bash
git init
git add .
git commit -m "Add Disaster Response Hub frontend reconstruction"
git branch -M main
```

5. Create an empty repository at <https://github.com/new>.
6. Copy its HTTPS URL and run (replace the sample URL):

```bash
git remote add origin https://github.com/YOUR-USERNAME/disaster-response-hub.git
git push -u origin main
```

If Git asks you to sign in, complete GitHub's authentication flow. Do not commit passwords, API keys, or `.env` secrets.

## Deploy the reconstructed static frontend

On Vercel, import the new GitHub repository. Since the project is plain HTML/CSS/JavaScript, no framework build command is needed. Set the output directory to the project root if prompted. This creates a new deployment; it does not replace or recover the original deployment unless you explicitly connect the appropriate project/domain.
