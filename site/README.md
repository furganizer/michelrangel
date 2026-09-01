# michelrangel.com

A static site — no build step required. Pages: `index.html`, `about.html`, `work.html`, `on-set.html`, `contact.html`.

## Deploy to Vercel

**Easiest path (no CLI):**
1. Go to vercel.com → New Project → Deploy → drag this whole `site` folder onto the page (or push it to a GitHub repo and import that repo).
2. Framework preset: choose **"Other"** (this is plain HTML/CSS/JS, no framework).
3. Leave the build command blank and set the output directory to `.` (project root).
4. Deploy — then connect your `michelrangel.com` domain under Project → Settings → Domains.

**Via CLI:**
```
npm i -g vercel
cd site
vercel
```
Follow the prompts (Other framework, no build command, output directory `.`).

## Updating content later
- Bio: edit the `<p>` tags in `about.html`.
- Credits: each title lives in a `.credit-row` block in `work.html` — copy/paste a block to add a new one.
- Posters: replace files in `assets/img/posters/` (keep the same filenames, or update the `src` in `index.html`).
- On Set photos: add new images to `assets/img/bts/` and add a matching `.gallery-item` block in `on-set.html`.
- Trailer: the Vimeo embed ID is in `index.html` inside the `<iframe src="...">` — swap the ID to change the video.

## Notes
- Fonts (Fraunces, Inter, IBM Plex Mono) load from Google Fonts via CDN — no local font files needed.
- Images have already been resized/compressed for web.
- Commercial and Music Video sections were intentionally left out of this first version — ready to add once those reels are ready.
