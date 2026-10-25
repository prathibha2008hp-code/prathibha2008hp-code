# Local profile preview

Preview the README in a browser before publishing:

1. From the repository root, start a local read-only file server:

   ```powershell
   python -m http.server 8000
   ```

2. Open [http://localhost:8000/preview.html](http://localhost:8000/preview.html).
3. Stop the server with `Ctrl+C` when you are finished.

The page loads `README.md` and its SVGs from this folder; it does not connect to GitHub to publish or change anything. It uses the Marked Markdown renderer from jsDelivr, so an internet connection is needed for the preview page. The README itself has no JavaScript.

The preview approximates GitHub's dark Markdown presentation. GitHub renders the README and local SVG images directly; the page styling, shadowed preview frame, and Markdown-rendering script are only for local preview.
