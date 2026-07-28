# Replace these two files in the repository root

Upload both files directly into the root of `bryannep/site`:

- `index.html`
- `style.css`

Do not place `style.css` inside `assets`, and do not replace the `assets` folder.

What was fixed:

- `index.html` now loads `style.css` from the repository root
- removed the broken `assets/script.js` reference; the required JavaScript is already embedded in `index.html`
- retained the centered Philosophy question rule
- retained “three ideas:” with the colon
- preserved all existing references to videos, images, PDFs, and icons inside `assets`

After GitHub finishes publishing, refresh the live page with Command + Shift + R.
