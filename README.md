# Neon Coast — 9-Panel Cover Studio

[![make.fun](https://make.fun/badge/gta6-cover-art-01.svg)](https://make.fun/bounty/gta6-cover-art-01)
[![rank](https://make.fun/badge/gta6-cover-art-01/hqnsyhrn/gta6-cover-art-01/rank.svg)](https://make.fun/bounty/gta6-cover-art-01)
[![reward](https://make.fun/badge/gta6-cover-art-01/hqnsyhrn/gta6-cover-art-01/reward.svg)](https://make.fun/bounty/gta6-cover-art-01)

An offline web app that turns any photos into GTA 6-style multi-panel cover art, built for the
[make.fun bounty gta6-cover-art-01](https://make.fun/bounty/gta6-cover-art-01).

- **9-panel cover grid** (plus Hero + 8, Hero + 3, Full-Bleed, Tilted Snapshots and Classic Poster layouts)
- **Multi-photo**: upload your own photos or use the 8 built-in samples; crop and position each panel
- **6 colour grades**: Sunset, Neon Vice, Teal Night, Heat Wave, Gold Hour, Mono Noir
- **Bold lettering**: Anton title with a halftone title block, Pacifico subtitle, heat-meter stars and a badge ribbon
- **PNG export in 4 sizes**: 1080×1080, 1080×1350, 1920×1080 and 1080×1920 (story)
- **Undo / redo, shuffle, film grain and vignette** — everything runs offline in the browser; photos never leave your machine

## Try it

```sh
node serve.ts
# open http://localhost:8080
```

## Entry

`main.ts` (Node 22) copies `app/` and `screenshots/` to the output directory and writes
`dossier.json` with the vendored make.fun library, as the kit's starter does:

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts
```

All art and lettering is original (Anton and Pacifico under the SIL Open Font License, in
`app/fonts/`). No Rockstar Games logo, artwork or fonts. Sample photos were made with an
image model; the two `pier` / `boulevard` samples come from the make.fun kit and are free to use.
