# Research content

The Research page and the home-page Snapshots carousel are driven by text and image files in `public/research/` and `public/snapshots/`.

## Research entries

Research entries live in `public/research/` and are split into two groups:

- Questions: `questions1_label.txt`, `questions2_label.txt`, etc.
- Approaches: `approaches1_label.txt`, `approaches2_label.txt`, etc.

The number controls display order. The label after the underscore is descriptive and does not affect ordering.

Each entry can have a matching image with the same stem:

- `questions1_programmable-lattices.txt`
- `questions1_programmable-lattices.png`
- `approaches1_metasurface-modes.txt`
- `approaches1_metasurface-modes.jpg`

Allowed image formats include `.png`, `.jpg`, `.jpeg`, `.webp`, `.avif`, and `.svg`.

## Research text formatting

Use this format in each `.txt` file:

```txt
Entry title

Main paragraph displayed on the Research page.

Additional paragraphs can be added as separate blocks.

Home snippet: Optional short caption for snapshot cards.
```

The first block becomes the entry heading. Other blocks are displayed as body paragraphs on the Research page. A paragraph beginning with `Home snippet:` is also used as the short caption for matching home-page snapshot cards.

## Snapshots carousel

Snapshot images live in `public/snapshots/`. No binary placeholder images are committed; add real images manually when ready. Use names such as:

- `questions1_snapshot_lattice.png`
- `questions2_snapshot_phases.jpg`
- `approaches1_snapshot_modes.webp`

Snapshot files include the matching research entry prefix, followed by `_snapshot_`, followed by any descriptive label. The carousel finds the matching research text from the prefix, uses that entry's title and optional `Home snippet:` caption, and links to the corresponding Research page card.

Snapshot order is randomized when the site is built or rendered, rather than following the question or approach numbering.
