This are the files for the nic cage film fest

## Favicon

The site icon is a stylized caricature of Nic Cage (`favicon.svg` is the source
artwork; the raster sizes are generated from it).

- `favicon.ico` — 16/32/48px, auto-requested by browsers at the site root
- `favicon.svg` — scalable, used by modern browsers
- `favicon-16x16.png`, `favicon-32x32.png`
- `apple-touch-icon.png` — 180px, iOS home screen

Once there is an HTML page, link them in its `<head>`:

```html
<link rel="icon" href="/favicon.ico" sizes="any">
<link rel="icon" href="/favicon.svg" type="image/svg+xml">
<link rel="apple-touch-icon" href="/apple-touch-icon.png">
```

## Lockstreak (`/tracker/`)

A small installable web app that tracks sobriety ("days since") counters and
daily habits, and renders the streak as a lock screen wallpaper sized for the
Pixel 10 (1080 × 2424). Live at `/tracker/` once deployed.

- No backend: everything is stored in the browser's localStorage, with JSON
  export/import for backups.
- `index.html` + `app.js` are the whole app; `sw.js` and `manifest.webmanifest`
  make it installable and usable offline.
- The PNG icons are rendered from `icon.svg` (192, 512, and a maskable 512).
- The wallpaper is a still image, so the count refreshes when you open the app
  and share or download it again.
