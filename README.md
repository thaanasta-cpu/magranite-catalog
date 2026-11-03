# Magranite Digital Catalog

## Setup
1. Create a **public** GitHub repository, e.g. `magranite-catalog`.
2. Upload `index.html`, `catalogs.json` and the `catalogs/` folder.
3. Add your actual PDFs in `catalogs/` named `tenax.pdf` and `lantania.pdf`, or change `catalogs.json` to match your filenames. Remove entries for catalogs you have not uploaded yet.
4. GitHub repository → Settings → Pages → Build and deployment → Deploy from a branch → `main` / `(root)` → Save.
5. Wait for GitHub Pages to publish. Your URL will resemble `https://USERNAME.github.io/magranite-catalog/`.

## Share a specific page
`https://USERNAME.github.io/magranite-catalog/?catalog=tenax#page=24`

The **Copy link** button creates a link for the current catalog and page.

## Add more catalogs
Upload `catalogs/newcatalog.pdf` and add an object to `catalogs.json`, e.g.:
`{"id":"newcatalog","title":"New catalog","file":"catalogs/newcatalog.pdf"}`

## Notes
- PDFs are **publicly accessible**; do not upload confidential pricing or private documents.
- GitHub rejects files larger than 100 MiB through ordinary Git uploads; browser upload limits may be lower. Optimize large PDFs first.
- PDF.js is loaded from cdnjs; the viewer requires internet access.
- PDF pages are rendered in a canvas; the interface supports page navigation, zoom, downloading and shareable page links, but not full-text search.
- This is a static site: no server or subscription is required. GitHub Pages availability and usage policies apply.
