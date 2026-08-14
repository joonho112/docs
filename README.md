# docs

Preprints and slides, served at <https://joonho112.github.io/docs/>

Everything here is temporary. Each preprint moves to arXiv eventually; this site
just gives it a shareable link in the meantime.

## Add an item

1. Copy `_template/` to `preprints/<slug>/` (or `slides/<slug>/`)
2. Drop in the PDF, edit the title, byline, abstract, and filename in `index.html`
3. Push

The link is `https://joonho112.github.io/docs/preprints/<slug>/`

**Share the folder URL, never the PDF directly.** A folder can be redirected
later; a PDF cannot.

## When it goes to arXiv

Replace `index.html` with:

```html
<!doctype html>
<meta name="robots" content="noindex">
<meta http-equiv="refresh" content="0; url=https://arxiv.org/abs/XXXX.XXXXX">
```

Old links keep working.

## Notes

- Folder names are permanent — renaming breaks links already shared.
- No Git LFS. Pages serves the pointer file, not the PDF.
- Submitted versions only, not publisher PDFs.
