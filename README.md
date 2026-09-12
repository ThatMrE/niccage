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
