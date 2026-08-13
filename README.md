# Presentation Imagery

Public asset host for the [EventPipe slide design
system](https://github.com/epprestodesign/presentation-templates), served over
GitHub Pages at:

**https://epprestodesign.github.io/presentation-imagery/**

## What is here

| Path | Contents |
|---|---|
| `imagery/unsplash/` | Stock photography, credited in [`credits.json`](credits.json) |
| `imagery/` | Backgrounds, covers, mosaics, product and value imagery |
| `team/` | Team headshots |
| `partners/`, `employers/`, `events/` | Partner, employer and event marks |

## What is deliberately NOT here

- **`references/slide-decks/`** — the original decks. They never leave the
  authoring machine.
- **`imagery/operating-layer-flattened/`** — photographs with a slide's scrim
  and title composited into the pixels. They are pictures of finished slides, so
  publishing them would publish deck copy. Excluded by path, not by filter, so a
  new file added there cannot slip out.

## How it is consumed

The design system resolves assets **locally first** and falls back to this host
for anything not on disk. That ordering matters: the PNG, PPTX and PDF exports
keep working offline and byte-identical, while the deployed Storybook still
shows its imagery.

Attribution for stock photography travels with the files in `credits.json`, as
the Unsplash API guidelines require.
