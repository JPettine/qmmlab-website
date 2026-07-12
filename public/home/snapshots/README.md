# Home research snapshots

Place snapshot images here to populate the home-page Research snapshots carousel.

## Naming convention

Use one of these patterns:

```text
questions1_snapshot_label.jpg
approaches1_snapshot_label.jpg
```

- `questions` or `approaches` connects the snapshot to the corresponding Research page section.
- The number links the snapshot to the matching Research card anchor, such as `/research/#questions1` or `/research/#approaches1`.
- `_snapshot_` is required.
- The filename label can be any descriptive text and does not affect display order. The carousel display label comes from the first non-empty line of the matching `public/research/questionsX_label.txt` or `public/research/approachesX_label.txt` file.

## Ordering

Snapshots are randomized when the site is built, so carousel order does not follow the question or approach numbering.

## Allowed image types and dimensions

Allowed image types are `.jpg`, `.jpeg`, `.webp`, `.avif`, `.gif`, and `.svg`. Do not add `.png` snapshots here; use `.jpg` for snapshot photos/exports.

Use landscape images close to **16:10** or **3:2**. The carousel uses a fixed image frame with `object-fit: cover`, so very tall or very wide images may be cropped.

## Carousel text

For each snapshot, the carousel label is read from the first non-empty line of the matching research text file. The descriptive snippet is read from the last line in that file that starts with `Home snippet:`; the prefix is not displayed.
