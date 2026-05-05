# Alpinism Training Plan

A 6-week training plan to build mountain fitness from a flatland base, designed for an alpinism course on June 14–19.

Live page: a single self-contained `index.html` with no build step and no dependencies.

## Hosting on GitHub Pages

1. **Create a new repository** on GitHub. Name it whatever you like (e.g. `alpinism-plan`). Public is required for free GitHub Pages.

2. **Upload `index.html`** to the root of the repo. Easiest way: click "Add file" → "Upload files" on the GitHub web UI and drop `index.html` in.

3. **Enable Pages**:
   - Go to the repo's **Settings** tab
   - In the left sidebar, click **Pages**
   - Under "Build and deployment", set **Source** to `Deploy from a branch`
   - Set **Branch** to `main` and folder to `/ (root)`
   - Click **Save**

4. **Wait ~1 minute**, then refresh the Pages settings page. You'll see a URL like:
   `https://<your-username>.github.io/<repo-name>/`

That's it — the page is live.

## Custom domain (optional)

In repo Settings → Pages, add your custom domain in the "Custom domain" field and add a `CNAME` DNS record pointing to `<your-username>.github.io`.

## Editing the plan

Everything is in one file. To update the weekly schedule, edit the `weeks` JavaScript object near the bottom of `index.html` — the structure is straightforward (theme, meta, days, key workout). Push to the `main` branch and Pages redeploys automatically in a minute.

## Features

- Fully self-contained, no external dependencies (no analytics, no fonts loaded from CDNs)
- Light and dark mode based on system preference
- Responsive on mobile
- Print-friendly (all weeks expand when printing)
