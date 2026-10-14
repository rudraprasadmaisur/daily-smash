# The Daily Smash — Archives

A complete illustrated timeline of one friend group's slow descent from a badminton net dispute
into empires, cartels, chess trophies and a dog in a party hat.

## Run locally
Just open `index.html` in a browser. No build step, no dependencies.

## Host on GitHub Pages
1. Create a new repo on GitHub (e.g. `daily-smash`).
2. Upload everything in this folder (`index.html`, `img/`, `README.md`) to the repo root.
3. Go to **Settings → Pages**.
4. Under *Source*, choose **Deploy from a branch** → branch `main`, folder `/ (root)`.
5. Save. In about a minute the site is live at:
   `https://<your-username>.github.io/<repo-name>/`

Or from the command line:

```bash
git init
git add .
git commit -m "The Daily Smash archives"
git branch -M main
git remote add origin https://github.com/<your-username>/<repo-name>.git
git push -u origin main
```

Then enable Pages in Settings as above.

## Adding a new event
Open `index.html`, find the `<div class="timeline" id="tl">` block, and copy an existing
`<article class="ev">` card. Change the date, tag, edition number and copy.

- Add `big` to the class (`class="ev big"`) to mark it as a headline event (solid timeline dot).
- The `data-t` attribute controls filtering. Valid values:
  `badminton`, `cards`, `food`, `trips`, `party`, `scandal` — space-separated, multiple allowed.
- Photos go in `img/` and are referenced as `<img src="img/yourfile.jpg">`.

## Notes
- Light and dark themes, toggled from the top-right button; the choice is remembered per browser.
- Fully responsive — works on phones.
- Everything is in one HTML file. No framework, no tracking, no cookies.
