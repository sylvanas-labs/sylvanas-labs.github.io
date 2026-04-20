# sylvanas-labs.github.io

Org site for [Sylvanas Labs](https://github.com/sylvanas-labs). Serves static content via GitHub Pages at `https://sylvanas-labs.github.io/`.

## What lives here

### `tiresias/index.json` — VPM package index for Tiresias

Consumed by the VRChat Creator Companion (VCC) and the `vpm` CLI. Register it in VCC with:

```
Settings → Packages → Add Repository → https://sylvanas-labs.github.io/tiresias/index.json
```

Or from the CLI:

```
vpm add repo https://sylvanas-labs.github.io/tiresias/index.json
```

**Source of truth:** Tiresias's source code and the canonical `index.json` are produced by the [sylvanas-labs/pantheon](https://github.com/sylvanas-labs/pantheon) monorepo at `tiresias/`. Releases of Tiresias trigger a workflow that updates this index file. If you're looking to contribute to Tiresias, work against that repo — this one is a thin hosting shell.

## Why this repo exists

GitHub Pages on a private repo requires a paid plan tier we don't have. The Pantheon monorepo is private. This public repo exists solely to serve the VPM index and any other static listing we want at stable `sylvanas-labs.github.io/<path>` URLs.

## History

The VPM index previously lived in the standalone `sylvanas-labs/tiresias` repo (archived 2026-04-20) as the root `index.json` file. When Pantheon absorbed Tiresias as a monorepo component, the hosting was migrated here.
