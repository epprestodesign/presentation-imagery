# Presentation Imagery

Public image host for the [EventPipe slide design
system](https://github.com/epprestodesign/presentation-templates). Served over
GitHub Pages at:

**https://epprestodesign.github.io/presentation-imagery/**

## What is here

Unsplash photography only — 153 photos across the subjects EventPipe decks need
pictures of. Every one is credited in [`credits.json`](credits.json) with the
photographer's name and profile link, as the Unsplash API guidelines require.

## What is deliberately NOT here

- **Original deck artwork.** EventPipe's own compositions, which carry company
  figures.
- **Staff headshots.** Photographs of real people are not ours to publish to a
  public CDN.
- **Partner, employer and event marks.** Third-party trademarks; using one on a
  private slide is not the same as republishing it from our own domain.

Those stay on the machines that need them and are gitignored in the design
system repo. This split is the reason this repo exists at all.

## How it is consumed

`img()` in the design system resolves local files first and falls back to this
host for anything not on disk — so exports stay offline and byte-identical,
while the deployed Storybook still shows its photography.
