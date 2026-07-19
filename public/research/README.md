# Research content and images

Research entries are generated from text files in this folder. Optional images can be added later using the same base file name as the matching text file.

## Naming convention

Research topic text files:

```text
topic1_label.txt
topic2_label.txt
```

Experimental approach text files:

```text
approaches1_label.txt
approaches2_label.txt
```

- The number controls display order and the page anchor (`topic1`, `approaches1`, etc.).
- The label can be any descriptive text and does not affect ordering.
- Optional images use the same base name with an allowed image extension, for example `topic1_label.png` or `approaches2_label.jpg`.

## Text formatting

```text
Entry title

First paragraph.

Second paragraph.

Home snippet: Short home-page carousel description.
```

The first paragraph block becomes the card title. Later paragraph blocks become justified body text. For home-page snapshots, the carousel label is the first non-empty line of the matching research text file, and the descriptive snippet is the last line that starts with `Home snippet:` with that prefix removed.

## Image formats and dimensions

Allowed image types are `.png`, `.jpg`, `.jpeg`, `.webp`, `.avif`, `.gif`, and `.svg`.

Images are displayed beside the text on larger screens, using about **1/3** of the card width for the image and **2/3** for text. Use a landscape image close to **4:3** to minimize cropping.
