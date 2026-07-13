# Personal Website

A single-page personal site — plain HTML + CSS with one tiny line of
JavaScript (it only fills in the year in the footer). No frameworks, no
build step, no dependencies. Easy to edit, free to host.

## Files

| File          | What it is                                            |
|---------------|-------------------------------------------------------|
| `index.html`  | **All your text and links live here.** Edit this.     |
| `styles.css`  | The look (colours, spacing, fonts). Rarely needs edits.|
| `README.md`   | This file.                                            |

## Editing your content

Open **`index.html`** in any text editor. Everything you'd want to change
is marked with a comment like:

```html
<!-- EDIT -->
```

- **Your name / tagline** — near the top, in the header.
- **Your bio** — look for the big `BIO PLACEHOLDER` block and replace the
  bracketed text with 2–4 sentences.
- **Social links** — find the `href="#"` values and paste in your real
  LinkedIn / Substack URLs. Replace `you@example.com` with your email in
  both the header and the Contact section.
- **Research / Writing / Industry entries** — each item is a list `<li>`.
  Change the text, or add/remove a line by copying an existing `<li>...</li>`.

To add a link to any item, wrap the text like this:

```html
<li><a href="https://the-url.com" target="_blank" rel="noopener">The title</a></li>
```

### Adding a photo (optional)

1. Drop an image named `portrait.jpg` in this folder.
2. In `index.html`, find the commented `<!-- OPTIONAL PHOTO -->` line inside
   the intro and remove the `<!--` at its start and `-->` at its end.

### Changing colours

Open `styles.css`. At the very top, in the `:root` block, are a handful of
colour variables (`--ink`, `--paper`, `--accent`, …). Change those values to
restyle the whole page. `--accent` is the single highlight colour used on
link hovers.

## Preview locally

Just double-click `index.html` — it opens in your browser. That's it.

If you'd prefer a local web server (optional), from this folder run:

```bash
python3 -m http.server 8000
```

then visit <http://localhost:8000> in your browser.

## Deploy free on GitHub Pages

1. Create a free account at <https://github.com> if you don't have one.
2. Make a new repository. To get a `username.github.io` address, name the
   repo exactly `your-username.github.io`. (Any name works; that one just
   gives the cleanest URL.)
3. Upload these files (`index.html`, `styles.css`, `README.md`) to the repo
   — you can drag-and-drop them via **Add file → Upload files** on the
   GitHub website, then **Commit**.
4. In the repo, go to **Settings → Pages**.
5. Under **Build and deployment → Source**, choose **Deploy from a branch**,
   pick the `main` branch and the `/ (root)` folder, and click **Save**.
6. Wait a minute, then reload the page — GitHub shows the live URL at the top
   (e.g. `https://your-username.github.io/`).

To update the site later, edit the files and upload/commit again; the live
site refreshes automatically within a minute or two.
