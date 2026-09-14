# Laplace EPUB Files

This repository contains the EPUB file structure for "Pierre Simon Laplace: 1749-1827; A Determined Scientist" by Roger Hahn.

## Files Uploaded

The following EPUB structure has been uploaded:

```
laplace_epub/
├── mimetype
├── META-INF/
│   └── container.xml
└── OEBPS/
    ├── content.opf
    ├── toc.ncx
    ├── book.xhtml
    └── css/
        └── style.css
```

## How to Create the EPUB File

To create a valid EPUB file:

1. Download all files from this repository
2. Create a ZIP archive with the following structure:
   - The mimetype file must be the first file in the ZIP archive
   - The mimetype file must NOT be compressed (store it as-is)
   - All other files can be compressed normally

### Using the zip command (Linux/macOS):

```bash
# Create the EPUB file
zip -X laplace_epub.epub mimetype
zip -r laplace_epub.epub META-INF OEBPS
```

The -X flag ensures the mimetype file is not compressed.

### Using 7-Zip (Windows):

1. Create a new ZIP archive
2. Add mimetype first with "Store" compression method
3. Add all other files with normal compression
4. Rename the .zip file to .epub

## About the Content

The book content has been:
- Extracted from the original PDF using OCR
- Cleaned to remove page markers, image references, and other artifacts
- Converted from Markdown to XHTML format
- Formatted with proper headers and emphasis
- Footnotes are preserved in superscript format

The text is the complete biography of Pierre Simon Laplace by Roger Hahn, published by Harvard University Press in 2005.

## Repository

- Owner: glazgogabgolab
- Repository: laplace_epub
- Original PDF: Pierre Simon Laplace, 1749-1827; A Determined Scientist - Roger Hahn.pdf
