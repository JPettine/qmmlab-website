# Highlights assets

Highlight images and captions are paired by file name.

## Image dimensions

Use a wide landscape image close to **16:9**. The home-page highlight carousel displays each image in a fixed landscape frame with `object-fit: cover`, so images far from 16:9 may be cropped.

## Allowed image types

Use common web image formats: `.png`, `.jpg`, `.jpeg`, `.webp`, `.avif`, `.gif`, or `.svg`.

## Naming convention

Each highlight image must be named:

```text
highlight1_label.png
```

- `highlight` is required.
- `1` controls display order. Use `highlight2_...`, `highlight3_...`, etc. for later slides.
- `_label` can be any descriptive label and does not affect ordering.
- The image extension can be any allowed image type.

The matching text file must use the same order number and label:

```text
highlight1_label.txt
```

## Text formatting and links

The text file is displayed as:

```text
Title shown in bold

Caption or description shown below the title.

https://example.com/link-target
```

- The first block is the bold highlight title.
- Middle block(s) become the description text.
- If the final block is a URL beginning with `https://`, `http://`, or `/`, the highlight image links to that destination.
