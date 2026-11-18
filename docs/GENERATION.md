# Overall generation process

The project reconstructs both the appearance of nineteenth-century type and
an editable, readable edition of the book. Michael Koksharov directed the work
through multiple cycles of ChatGPT 6 Work, comparing generated material with
the historical scans and specifying typographic corrections.

## Typeface reconstruction

### Reference selection

The main Latin source is the first-edition *Origin of Species* scan held by
Wellcome Collection. Repeated impressions of a letter are compared so that
a broken stroke, ink spread, pencil mark, or scanning defect is not treated
as an intended part of the design. Italic words, headings, punctuation, and
catalogue text supply additional examples.

### Outlines and proportions

Scan-derived contours are converted into scalable outlines. Local tracing
and Bézier redrawing preserve characteristic proportions, stroke contrast,
serifs, counters, and terminals. Straight edges and sharp crossings are kept
as explicit geometry where the print supports them. Baselines, capital heights,
curve overshoot, and serif treatment are checked for consistency without
forcing every letter into a generic modern design.

### Companion forms and Greek

A dedicated small-caps face is constructed from the regular design at a
height comparable to lowercase letters, with adjusted widths and weight.
Supplemental accents, punctuation, and slanted numerals are fitted to the
existing design.

The Greek extension uses the alphabet and repeated examples in Kühner’s 1859
grammar, particularly printed pages 15–22. The work includes local source
tracing and explicit line and curve constructions. Slanted source forms are
adapted into an upright companion where necessary, then matched to Origin’s
scale, weight, and spacing. Modern functional additions, such as the distinct
micro sign, are distinguished from historically attested source forms.

### Spacing and packaging

Sidebearings and kerning are reviewed in words, enlarged proofs, reading-size
text, and the Cyreal and Typefacts test passages. Letter and punctuation pairs
are adjusted individually. OpenType positioning and legacy kerning tables
support applications with different shaping capabilities. The results are
packaged as Regular, Italic, and Small Caps TTF files, with linked family/style
names, embedding permissions, and author metadata.

## Book reconstruction

### Text and page references

Scan-derived text and page geometry are reconciled with the matching
first-edition transcription and images from Darwin Online. Historical spelling,
quotation marks, punctuation spacing, italics, superscripts, and small caps
are reviewed against the print. Duplicate scan leaves are removed, and missing
preliminary and body pages are reconstructed from another first-edition copy.

### Typesetting

The book is rebuilt as native DOCX text using the Origin fonts. Printed page
boundaries and many original line breaks are retained. Page sections, paragraph
formatting, consistent margins where suitable, justification, odd/even running
headers, and page fields reproduce the overall design. Title matter, contents,
index columns, catalogue entries, signatures, rules, and other special material
receive separate layout treatment. The folded diagram remains a scan image.

### PDF production and checking

The DOCX is rendered to PDF with embedded fonts. Compact fraction previews
receive invisible text values and ActualText for copying and searching; footer
reading order is repaired without changing visible ink. Text extraction,
page counts, line wrapping, clipping, index gutters, superscripts, and potential
text/rule collisions are checked. Rendered pages and enlarged details are
compared with the source.

These checks improve fidelity but do not establish a completely error-free
critical edition or an exact facsimile of every original impression. The PDF
preserves the supplied layout; another editor’s DOCX rendering can differ.

This repository distributes the finished book and font files with process
documentation. It does not include a complete, one-command build environment
for regenerating every glyph and page from the original scans.
