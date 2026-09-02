# Around the Cooler — Podcast Website

A simple static website for *Around the Cooler: The Fantasy Football Podcast*.
No build tools, no CMS — just `index.html` + `style.css` + a logo. Open
`index.html` in a browser and it works.

## Before you publish

- **Swap the logo.** `assets/logo-900.png`, `assets/logo-180.png`, and
  `assets/favicon-32.png` were generated from a Fiverr proof file that still
  has a faint watermark. Once you have the final delivered logo, re-export
  it at those same three sizes (or just replace the files and re-crop) and
  drop it in `assets/`, keeping the same filenames so nothing else needs to
  change.
- **Fill in host bios.** `index.html` has three placeholder bio lines under
  "Meet the Hosts" (search for `TODO`). Swap in real bios/photos when ready.
- **Instagram and Twitter/X are linked** in the footer
  (`atc.fantasyfootball` and `@AroundtcoolerFF`).
- **Confirm the Spotify link.** The "Listen on Spotify" button currently
  points at a Spotify search results page (it works, but isn't the direct
  show page) since I couldn't confirm your exact `open.spotify.com/show/...`
  URL. Open the show in the Spotify app, copy its share link, and swap it
  in — search for `TODO` in `index.html` to find the spot.

## Publishing with GitHub Pages (free hosting)

1. Create a new repository on GitHub (e.g. `around-the-cooler`). Don't
   initialize it with a README — this folder already has one.
2. From inside this folder, connect it to your new repo and push:
   ```
   git remote add origin https://github.com/<your-username>/around-the-cooler.git
   git push -u origin main
   ```
3. On GitHub, go to your repo's **Settings → Pages**.
4. Under "Build and deployment," set **Source** to "Deploy from a branch,"
   branch `main`, folder `/ (root)`. Save.
5. GitHub will give you a live URL, typically:
   `https://<your-username>.github.io/around-the-cooler/`
   (takes a minute or two to go live after the first push).

Every time you edit a file and want the live site updated, just run:
```
git add -A
git commit -m "describe your change"
git push
```
