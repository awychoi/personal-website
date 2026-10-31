# wychoi.com — public build log

The source is private. This repository is the public build log and the Workbench card.

## Build notes

- **Static runtime, dynamic build.** Owner's public Github repo data is collected and cached at build time; the Workbench cards and résumé PDF are prepared then. Visitors receive static files, and no request reaches GitHub on their behalf.
- **The résumé is an artifact.** A headless browser renders it during the build, and a fingerprint check refuses to publish a PDF that no longer matches the content. Nothing is rendered at request time.
- **Repo-owned cards.** A public repo can declare a hero card, grouped row, or hidden. The four-axis flip uses four stacked copies, one per axis; only the visible one is painted and animated, and the return switches to a different layer. Grouped rows can carry light/dark SVG icons. This repo's card lives in [`workbench.md`](workbench.md).
- **Small surface.** No CMS, database, server function, analytics, cookies, ads, newsletter, contact form, or third-party runtime. Assets are same-origin. The published site has no phone number, references, or private project links. If upstream data is unavailable, the last good copy is kept; a malformed card fails the build.

Static doesn’t mean simple. The hard parts were the artifact checks, the card state, and deciding what not to add.

## Live site

`wychoi.com`
