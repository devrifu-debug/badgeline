# Badgeline — ID Card Studio

Make ID cards in bulk from a spreadsheet, right in the browser.

**Live app:** https://devrifu-debug.github.io/badgeline/

## What it does

1. **Pick a template**: 27 ready-made designs (portrait, landscape, front & back, Bangla school ID and more), or upload your own design (PNG, JPG, SVG or PDF from Canva or Figma) and edit it.
2. **Import data**: Excel (.xlsx) or CSV. Photos placed inside the Excel cells are picked up automatically, or upload photos / a ZIP named by ID or name.
3. **Map fields**: columns are matched to card fields automatically; adjust if needed.
4. **Preview & fix**: validation flags missing names, duplicate IDs, bad emails and missing photos.
5. **Generate & export**: print-ready A4 PDF sheets (with cut marks and duplex backs), one PDF per card, or PNG/JPG images in a ZIP.

Everything runs locally in your browser. Spreadsheets and photos are never uploaded to a server. Templates and projects are saved in your browser's storage (IndexedDB).

## Run locally

It is a single static file. Open `index.html` in a browser, or serve the folder:

```bash
npx serve .
```

## Tech

React 18 + htm (no build step), canvas rendering engine, SheetJS, JSZip, jsPDF, pdf.js, qrcode-generator.
