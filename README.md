# AI Engineering Patterns in Python — reader

A static, GitHub Pages-ready reader for the complete PDF. The PDF in this folder is an exact copy of the original; the source PDF and Word document are untouched.

## Preview locally

Open a terminal in this folder and run:

```sh
python3 -m http.server 8000
```

Then visit <http://localhost:8000>. Use a local server rather than opening `index.html` directly: browsers restrict PDF and index loading from `file://` URLs. Stop the server with Ctrl+C.

## Publish on GitHub Pages

1. Create a GitHub repository and upload **all files and folders in this folder** to its root, including `libro.pdf`, `indice.json`, and `vendor/`.
2. Open `config.js` and replace the empty string with the repository URL, for example `https://github.com/your-username/your-repository`. This enables the **Star on GitHub** link. Replace the example with your actual URL.
3. In the repository, open **Settings → Pages**. Under **Build and deployment**, select **Deploy from a branch**, then choose your default branch and `/ (root)`, and save.
4. GitHub Pages will display the published URL in the Pages settings once deployment completes.

The site is static: no account, backend, or build step is required. Reading position and bookmarks are saved locally in each browser. Links like `#page=12` open a particular page. Search matches text extracted by PDF.js; extraction quality depends on the PDF. The reader loads its PDF rendering library locally; optional Google Fonts use a network connection and have local fallbacks. PDF.js is distributed under its bundled license in `vendor/LICENSE-pdfjs.txt`.

The index in `indice.json` was generated from the PDF's existing bookmarks. The PDF remains the definitive source for all content and page layouts.
