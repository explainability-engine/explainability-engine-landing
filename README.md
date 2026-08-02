# explainability-engine-landing

Source for the Explainability Engine landing page.

**Live site:** https://explainability-engine.github.io/explainability-engine-landing/

## What this repository is

A single static page (`index.html`) served by GitHub Pages. No build step, no
dependencies, no framework — HTML, CSS and a small amount of inline JavaScript
in one file. Edit `index.html`, push to `main`, and Pages redeploys.

This repository contains the marketing site only. The engine itself — the API
that produces the sealed audit bundles described on the page — lives in a
separate repository.

## What the product is

Explainability Engine is a deterministic, model-agnostic audit layer for AI
decision systems, delivered as an HTTP API. A client submits a structured
decision graph together with a context object; the engine returns a
cryptographically sealed bundle that can be re-derived bit-for-bit from the same
inputs and verified independently by a third party.

The engine does not make decisions, does not run language models, and does not
evaluate whether a decision was correct — only that the record of it is
structurally sound and has not been altered since it was sealed.

- API base: `https://explainability-engine-v1-production.up.railway.app`
- Health check (no auth): `GET /health`
- Patent pending P.455178 (UPRP, Poland, filed 23 March 2026)

## Local preview

```bash
python3 -m http.server 8000
# open http://localhost:8000
```

## Contact

Oleksandr Rudenko · JDG, Wrocław, Poland
[LinkedIn](https://www.linkedin.com/in/oleksandr-rudenko-24b061339)

## License

The page copy, design and product names are © 2026 Oleksandr Rudenko, all rights
reserved. This repository is public because GitHub Pages requires it; it is not
an open-source release.
