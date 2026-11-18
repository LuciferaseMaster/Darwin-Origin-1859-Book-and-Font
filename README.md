# Origin 1859 Book & Font

This project is an attempt to create an appealing, vintage-style digital font
for scientific writing and science hobby projects. Charles Darwin’s *On the
Origin of Species*—one of the most recognizable scientific books of the
nineteenth century—provides a natural starting point.

It is also an experiment in the capabilities of modern large language models:
I am using **ChatGPT 6** to streamline the process of reconstructing historical
letterforms and reproducing the book’s typography and layout.

The project currently includes a digital font family based on the **first
edition of Darwin’s *On the Origin of Species* (1859)** and a **compact PDF
reconstruction of the book typeset with these fonts**. An editable Word version
is also included.

Font design and reconstruction: **Michael Koksharov**, using multiple cycles
of **ChatGPT 6 Work**. Charles Darwin is the author of the original book.

![Origin 1859 Text: Regular, Italic, Small Caps, and sample Greek letters.](fonts/images/Origin1859-Overview.png)

## Download

| Material | File |
| --- | --- |
| Book for reading | [PDF](book/Darwin-Origin-1859-Text.pdf) |
| Editable book | [Word DOCX](book/Darwin-Origin-1859-Text.docx) |
| Regular font, 1.00 | [Origin1859-Regular.ttf](fonts/ttf/Origin1859-Regular.ttf) |
| Italic font, 1.00 | [Origin1859-Italic.ttf](fonts/ttf/Origin1859-Italic.ttf) |
| Small caps font, 1.00 | [Origin1859-SmallCaps.ttf](fonts/ttf/Origin1859-SmallCaps.ttf) |

The book has **544 PDF pages**, including the preliminary matter, folded
diagram and its reverse, main text, index, and publisher’s catalogue.
The DOCX embeds the same three fonts provided here. Install the TTF files
for editing, and use the supplied PDF for a fixed reading layout.

## About the reconstruction

Letterforms were recovered from scans, compared across repeated impressions,
and refined as vector outlines. Spacing and kerning were adjusted for readable
text while retaining the character of the source printing. The Greek letterforms
were reconstructed from the type used in Raphael Kühner’s Greek grammar
(1859), then adapted to match the Origin fonts.

The book combines scan-derived text with comparison against the first-edition
transcription and images. Its layout preserves printed page boundaries,
justification, running heads, italics, small caps, superscripts, rules, index
columns, and catalogue structure. Missing leaves were reconstructed from
another first-edition source. The folded diagram remains an image.

This is a historical reconstruction, not an exact recovery of the original
metal type or a fully proofread critical edition. Fine details and occasional
transcription or layout errors may remain.

## Documentation

- [Overall generation process](docs/GENERATION.md)
- [Book contents and editing notes](book/README.md)
- [Font installation, coverage, and design notes](fonts/README.md)
- [Sources and acknowledgements](docs/SOURCES.md)
- [Rights and included licenses](LICENSE.md)

[SHA256SUMS](SHA256SUMS) records the checksums of the repository’s files.
