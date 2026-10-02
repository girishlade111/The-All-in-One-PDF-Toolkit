# The All-in-One PDF Toolkit (PDF Power Tools)

A free, no-login, all-in-one PDF utility website — merge, split, rotate, compress, protect, and convert PDF files entirely in your browser. Files are processed 100% client-side, so nothing is ever uploaded to a server.

## Features

Organized into categories, the toolkit ships with 20 tools (4 fully implemented client-side, more planned):

**Organize & Edit**
- **Merge PDF** — combine multiple PDFs into one single document
- **Split PDF** — divide a PDF into multiple smaller documents (by range or per-page)
- **Rotate PDF** — rotate all or specific pages
- **Page Numbers** — insert page numbers into a PDF document
- *(Coming soon)* Organize pages, Edit PDF, Crop PDF

**Convert from PDF** (coming soon)
- PDF to Word / PowerPoint / Excel / JPG / PNG / Text

**Convert to PDF** (coming soon)
- Word, PowerPoint, Excel, JPG, PNG, and Text to PDF

**Security & Compress** (coming soon)
- Protect PDF (password), Unlock PDF, Compress PDF

**Extras**
- Dark mode toggle with persistent theme
- Modern Tailwind CSS UI with Lucide icons
- Fully responsive — works on mobile and desktop

## Tech Stack

- **Single `index.html`** — HTML5, Tailwind CSS (CDN), vanilla JavaScript
- **PDF manipulation:** [pdf-lib](https://pdf-lib.js.org/) (CDN)
- **File downloads:** FileSaver.js (CDN)
- **Archives:** JSZip (CDN)
- **Icons:** Lucide (CDN)

No build step, no dependencies to install, no backend.

## Quick Start

1. Clone or download this repository.
2. Open `index.html` directly in a browser, **or** serve it locally:
   ```bash
   npx serve .
   # then open http://localhost:3000
   ```
3. Pick a tool, drop in your PDF files, and download the result.

## Project Structure

```
The-All-in-One-PDF-Toolkit/
├── index.html   # The entire app: UI, tool registry, and all PDF logic
└── README.md
```

## Privacy

All processing happens locally in the browser via pdf-lib. No uploads, no accounts, no tracking.

## Deploy Notes

Pure static site — deploy anywhere static hosting works:
- **GitHub Pages:** branch `main`, path `/` → https://girishlade111.github.io/The-All-in-One-PDF-Toolkit/
- Any static host (Cloudflare Pages, Netlify, Vercel) — no build command needed.

## Contributing

New tools are defined in the `tools` array in `index.html` — add an entry with `id`, `name`, `description`, `icon`, `category`, and `implemented` flag, then implement the handler.

---

**Built by Girish Lade** — [ladestack.in](https://ladestack.in)
