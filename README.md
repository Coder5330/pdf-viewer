# Quickview

A browser-based PDF viewer and editor — view, annotate, OCR, search, fill forms, reorder pages, and export, all client-side with no server or accounts.

Owned by [Coder5330](https://github.com/Coder5330). Coded by Claude.

## Features

- View, zoom, and navigate multi-page PDFs
- Annotate with pen, highlighter, shapes, and text
- Reorder, rotate, duplicate, delete, and merge pages
- OCR scanned pages (via [Tesseract.js](https://github.com/naptha/tesseract.js)) to make them searchable
- Search text across the document, with word-level highlighting for both digital text and OCR results
- Word-processor-style text selection with copy-to-clipboard, shift-click range extend, and auto-scroll/auto-page-advance while dragging
- Detect and fill AcroForm fields (text, checkbox, dropdown, radio), flattened into the exported PDF
- Edit existing text in place — click a line to retype it; covers the original with its sampled background color and draws the new text on top (an approximation, not true reflow, since PDFs don't store editable paragraphs — the page is rasterized on export, same as any other annotation)
- Digitally sign a PDF with a real, client-side-generated X.509 certificate — a PAdES/CMS (`/Sig`, detached PKCS#7) signature that verifies in Adobe Reader and other standard validators, meeting eIDAS Advanced Electronic Signature and ESIGN Act bars (self-signed, or an imported CA-issued `.p12`; not eIDAS Qualified, which requires a licensed EU Trust Service Provider)
- Export the edited PDF, or print it

## Stack

Single-file static HTML app (`index.html`) built on [PDF.js](https://mozilla.github.io/pdf.js/), [pdf-lib](https://pdf-lib.js.org/), [Tesseract.js](https://github.com/naptha/tesseract.js), and [node-forge](https://github.com/digitalbazaar/forge) — no build step, no backend. Everything runs in the browser; nothing is uploaded anywhere.

## Source

https://github.com/Coder5330/pdf-viewer

## License

[MIT](LICENSE)
