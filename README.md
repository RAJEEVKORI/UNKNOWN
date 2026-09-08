# PagePress

A single-file, browser-based tool for compressing, merging, trimming, and signing PDFs and images — including presets for Indian competitive exam form uploads (IBPS, SSC CGL, UPSC, RRB).

**100% local.** Everything runs client-side in your browser via JavaScript. No files are ever uploaded to a server — there is no backend at all. Results are only ever available as a direct download to your device.

## Features

- **Compress** — shrink an image or PDF to:
  - a target file size (KB/MB)
  - target pixel dimensions
  - an **exam form spec** preset (auto-fills the pixel size and KB range for IBPS/SSC CGL/UPSC/RRB photo & signature uploads, then crops/scales to the exact box)
- **Merge** — combine multiple PDFs in a chosen order, optionally forcing a uniform output page size (A4/Letter/Legal/A3)
- **Remove pages** — thumbnail picker to drop specific pages from a PDF
- **Sign** — draw a signature or upload a signature image, drag/resize it onto any page, and bake it into the PDF

## Usage

Just open `pagepress.html` in any modern browser (Chrome, Edge, Firefox, Safari). No build step, no install, no dependencies to set up locally — it pulls `pdf-lib` and `pdf.js` from a CDN at runtime.

## Tech

Single HTML file — vanilla JS, [pdf-lib](https://pdf-lib.js.org/) for PDF creation/editing, [pdf.js](https://mozilla.github.io/pdf.js/) for rendering pages to canvas.

## Disclaimer

Exam board photo/signature specifications change between notification cycles. The exam presets reflect commonly published figures at the time of writing — always confirm the exact KB range and pixel dimensions in your current official notification before submitting an application.

## License

MIT
