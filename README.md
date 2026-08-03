# geopages-preview

Public **noindex** preview of the Blip Texas geo location-page prototype.

- **Live:** https://jmunnerlyn.github.io/geopages-preview/billboard-locations/texas/
- **Houston:** https://jmunnerlyn.github.io/geopages-preview/billboard-locations/texas/houston-tx/
- **Addison (near-city):** https://jmunnerlyn.github.io/geopages-preview/billboard-locations/texas/addison-tx/
- **Source:** Blip geopages prototype (`build.py --preview` → static `dist/`)
- **Indexing:** Disabled (`robots.txt` Disallow, `noindex` meta, preview banner). Internal team share only.
- **Contents:** Built static files only — not the monorepo, not secrets, not source pipelines.
- **Production host (later):** marketing site Astro repo (`blipbillboards.com`) — this preview is not that cutover.

## Refresh

From the geopages prototype:

```bash
./prototype/deploy-github-pages.sh
```

That rebuilds with `--preview`, copies `prototype/dist` into this repo (plus `.nojekyll` + this README), commits, and pushes to `main`.

**One-time Pages setup** (if the live URL 404s): repo **Settings → Pages → Build and deployment → Source: Deploy from a branch → Branch: `main` / `/ (root)` → Save**.

Do not commit `.env`, Redshift credentials, or the private monorepo into this repository.
