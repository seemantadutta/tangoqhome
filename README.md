# Landing page

Static landing page for the Tango Mode for Mixxx fork. Plain HTML/CSS, no build step.

Design: a "golden-age tango record label" look - gold-on-wood, Playfair Display
headings, Inter body, aged-parchment text, and a single deep tango red as the
accent. Theme tokens live in the `:root` block of `styles.css`.

## Preview locally
Open `index.html` in a browser, or serve the folder:
```
python -m http.server 8000
# then visit http://localhost:8000
```

## Publish with GitHub Pages
Settings > Pages > Source: **Deploy from a branch** > branch `main`, folder
`/docs`. The site will be at `https://<user>.github.io/<repo>/`.
(For a cleaner URL you can instead move these files into a dedicated repo, e.g.
`tango-mode`, and serve from its root or `/docs`.)

A custom domain later is just a `CNAME` file in this folder plus a DNS record.

## Fill these in before sharing (search for `TODO` / `YOUR_`)
- **YouTube** tutorial/channel URL (hero + `youtube.com/@YOUR_CHANNEL`).
- **GitHub Release** URLs for the Windows `.msi` and macOS `.dmg`.
- **SHA-256 checksums** for each installer (build trust for unsigned binaries).
- **PayPal.me** handle (`paypal.me/YOUR_HANDLE`).
- **Fork repo URL** / default branch and the **compare** URL vs upstream.
- **Build guide** path (currently `INSTALL.md`).
- `og:url` in the `<head>`.

## Branding & assets (already wired into the page)
- **Logo is a typographic wordmark** (no image): "Tango Mode for Mixxx" in
  Cormorant Garamond, "Tango" italic in red. Used in the hero and nav; edit it in
  the `.hero__wordmark` / `.brand` rules of `styles.css`.
- `favicon.svg` / `seal.svg` - the navy record-label disc mark (favicon + the small
  emblem shown beside the wordmark in the hero and nav).
- `tangomodemixxx_hero_screenshot.png` - full-window hero screenshot, also used as
  the `og:image` social card.
- Feature shots: `keep_queue.png`, `cortina_fades.png`, `set_length_and_time.png`,
  `live_mode_lock.png`, `always_visible_queue.png`, `live_cortina_nudge.png`.
- `tangomodeformixxx.png` - the original AI-generated logo, **no longer used**
  (left in assets; safe to delete). `wordmarks.html` is the throwaway compare page.

Optional polish:
- A dedicated `~1200x630` `og-preview.png` (e.g. the wordmark on the dark ground)
  is a sharper social card than the screenshot; point `og:image` at it if you make one.
- Some feature crops are small; higher-resolution crops look sharper where the
  layout shows them wide. A short **GIF of a cortina fade** is a great hero add.

## Note
The "unofficial fork / not affiliated with Mixxx" framing is in the banner and
footer by design. Keep it.
