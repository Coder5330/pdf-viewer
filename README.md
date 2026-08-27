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
- Export the edited PDF, or print it

## Stack

Single-file static HTML app (`index.html`) built on [PDF.js](https://mozilla.github.io/pdf.js/), [pdf-lib](https://pdf-lib.js.org/), and [Tesseract.js](https://github.com/naptha/tesseract.js) — no build step, no backend. Everything runs in the browser; nothing is uploaded anywhere.

## Source

https://github.com/Coder5330/pdf-viewer
