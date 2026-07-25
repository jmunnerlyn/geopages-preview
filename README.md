# geopages-preview

Public **noindex** preview of the Blip Texas geo location-page prototype.

- **Live:** https://jmunnerlyn.github.io/geopages-preview/billboard-locations/texas/
- **Source:** Blip geopages prototype (`build.py --preview` → static `dist/`)
- **Indexing:** Disabled (`robots.txt` Disallow, `noindex` meta, preview banner). Internal team share only.
- **Contents:** Built static files only — not the monorepo, not secrets, not source pipelines.

## Refresh

From the geopages prototype:

```bash
./prototype/deploy-github-pages.sh
```

That rebuilds with `--preview`, copies `prototype/dist` into this repo, commits, and pushes to `main`. GitHub Pages serves from `main` / root.

Do not commit `.env`, Redshift credentials, or the private monorepo into this repository.
