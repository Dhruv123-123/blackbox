# Blackbox

An aviation accident knowledge graph with a flight-data-recorder replay, a cockpit
audio track, a globe of every accident on record, documentary story mode and
FlightGear export. Everything runs in the browser; the data is in `blackbox/`.

```
npm install
npm run dev        # http://localhost:5173
npm run build      # static site in dist/
```

Method, data schemas and the pipelines are documented in [blackbox/README.md](blackbox/README.md)
and [blackbox/SPEC.md](blackbox/SPEC.md).

## Put it online for free (GitHub Pages)

1. Create a **public** GitHub repository named `blackbox` and push this tree to its `main` branch.
2. In the repository's Settings → Pages, set "Build and deployment → Source" to **GitHub Actions**.
   (The workflow token cannot turn Pages on by itself; this is a one-time click.)
3. The included workflow (`.github/workflows/pages.yml`) builds the app with `BASE_PATH=/blackbox/`
   and deploys `dist/` on every push to `main`. Re-run it from the Actions tab after step 2.
4. It is then served at `https://<your-user>.github.io/blackbox/`. Add a custom domain under
   Settings → Pages if you want it on your own domain.

For a root deployment (any static host, or a repository named `<user>.github.io`), leave `BASE_PATH` unset.

## License

MIT for the code. Accident records are derived from public investigation reports and
Wikipedia; recordings come from Wikimedia Commons under the licence stated on each.
