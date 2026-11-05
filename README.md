# SIAM Chapters Meeting 2027 – website

A static website for GitHub Pages. No build step, no Node, no React: just upload the files.

## Files

| File | What it is |
|---|---|
| `index.html` | The website. You never need to edit it. |
| `content.js` | **All the text, dates, speakers, schedule, logos…** The site reads everything from here. |
| `editor.html` | A visual editor for `content.js`, with a live preview. |
| `logos/`, `speakers/`, `people/`, `downloadables/` | Images and PDFs used by the site. |

## Publish on GitHub Pages (once)

1. Create a repository (e.g. `siam-cm-2027`) and upload all these files, keeping the folders.
2. Go to **Settings → Pages**, choose **Deploy from a branch**, branch `main`, folder `/ (root)`, and save.
3. After a minute the site is live at `https://<organisation>.github.io/<repository>/`.

## Update the content

1. Download the repository (or keep a local copy of these files) and double-click **`editor.html`**.
2. Fill in dates, venue, speakers, schedule, etc. The preview on the right updates as you type,
   and your work is kept in the browser until you download it.
3. Click **Download content.js**.
4. On GitHub: **Add file → Upload files**, drop the new `content.js` (it replaces the old one), and commit.
   Upload any new photos to `speakers/` or `people/`, and logos to `logos/`, the same way.

Empty fields show "To be announced" on the site, so you can publish now and fill things in later.

### Handy details

- In text fields you can write `**bold**`, `*italic*` and `[link text](https://…)`.
- `{year}`, `{dates}`, `{venue}` and `{location}` are replaced automatically with the values from the *General* and *Venue* pages.
- Keynote abstracts support LaTeX maths between `$…$`.
- Colours: the *Colours* page in the editor sets the whole palette (light and dark mode are derived automatically).
- Sections can be hidden from *General → Visible sections* (e.g. hide *Talks and posters* until the list is ready).
- For the map: Google Maps → *Share* → *Embed a map* → copy only the link inside `src="…"`.
- `editor.html` only edits files on your computer; it is harmless if it is also online. You can delete it from the repository if you prefer.

## Still to add for UniGe

- `logos/unige.png` and a DIMA logo, then set them in *Institutions → Contributors* (they show as text tiles until then).
- The chapter contact email (*Venue and travel → Contact*) and, if you have one, a privacy policy PDF (*Footer*).
