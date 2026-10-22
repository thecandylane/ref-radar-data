# ref-radar data

The nightly export of [ref-radar](https://ref.lookit.space), a curated prior-art index for coding agents: who already built this, where to start reading, and whether you can reuse it. The live catalog is at ref.lookit.space. This repo is a copy of it, refreshed every night, so it is also the backup and the fallback when the site is down.

## Files

- `catalog.json`: every live ref, one per line, with its why line, keys, facets and a stats summary.
- `taxonomy.json`: the domains, races and capabilities, with aliases.
- `r/{idpath}.json`: full records with start-here paths, a fetch recipe pinned to a commit, and facts. The idpath is the id with its first colon turned into a slash, so `gh:owner/repo` becomes `gh/owner/repo`.

The paths match the site's, so `https://raw.githubusercontent.com/thecandylane/ref-radar-data/main/catalog.json` is the same file as `https://ref.lookit.space/catalog.json` as of the last export.

These files are generated from the live catalog. A pull request that edits them would be overwritten by the next export.

## Suggest a ref

Open an issue with the **Submit a ref** form and give a GitHub repository or an arXiv paper. A daily job adds it to the review queue and comments on the issue. The issue closes when the suggestion is accepted or turned down. Every ref is reviewed by hand before it is listed.
