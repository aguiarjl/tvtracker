# TV Tracker

A personal watch tracker for TV shows and movies. Tracks status, ratings, episode-level watch history, and checks TMDB for new aired episodes on shows you're watching. Links out to IMDb for each title.

## Local development

```
npm install
npm run dev
```

## Deploy to GitHub Pages

1. Create a new repo on GitHub and push this folder to it (branch `main`).
2. In the repo, go to **Settings > Pages**, and under "Build and deployment" set **Source** to **GitHub Actions**.
3. Push to `main` (or re-run the workflow from the **Actions** tab). The included workflow (`.github/workflows/deploy.yml`) will build and publish automatically.
4. Your app will be live at `https://<your-username>.github.io/<repo-name>/`.

Every future push to `main` redeploys automatically.

## TMDB API key

Add your own free TMDB API key inside the app (gear icon). It's stored in your browser's local storage on the deployed site, not committed to the repo.

## Data storage

All your entries, watch history, and API key are stored in your browser's local storage. This means:
- Your data stays private to your device and browser
- Clearing browser data/cache will erase it
- It does not sync across devices
