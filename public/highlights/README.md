# Highlights content

Highlight slides are loaded from this folder and ordered by the number in each file name.

## Image dimensions

Use a wide image ratio of **16:7** for undistorted display in the home-page carousel. The site crops images with `object-fit: cover` so nearby ratios still work, but 16:7 avoids unexpected edge cropping.

## Allowed image file types

Compatible web image formats are supported, including `.png`, `.jpg`, `.jpeg`, `.webp`, `.avif`, and `.svg`.

## File naming

Each highlight needs a matching image and text file:

- Image: `highlight1_label.png`
- Text: `highlight1_label.txt`

The number controls the carousel order. The label after the underscore is for your own description and does not affect ordering. The image extension can be any allowed image type, but the text file must use the same stem and end in `.txt`.

Examples:

- `highlight1_vectorcurrents.png`
- `highlight1_vectorcurrents.txt`
- `highlight2_group-photo.jpg`
- `highlight2_group-photo.txt`

## Text file formatting

Use this format:

```txt
Slide title

Short descriptive paragraph shown in the hover caption. Additional paragraphs are joined into the same caption text.

https://example.com/article-or-page
```

The first non-empty block is displayed as the bold header. Remaining text is displayed as the caption body, except for the final link line. If the last non-empty line starts with `http://`, `https://`, or `/`, the highlight image links there. External links open in a new tab; internal links use the same tab.
