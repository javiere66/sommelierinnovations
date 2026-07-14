# Sommelier Innovations — Menús Digitales

Digital, mobile-first menus for our bars, served free via GitHub Pages and
reachable by QR code at each table.

## Live site

- **Landing (all bars):** https://javiere66.github.io/sommelierinnovations/
- **Palapa Bar menu:** https://javiere66.github.io/sommelierinnovations/bars/palapa-bar/
- **Palapa Bar printable QR:** https://javiere66.github.io/sommelierinnovations/bars/palapa-bar/qr.html

## Structure

```
.
├── index.html              Landing page listing every bar
└── bars/
    └── palapa-bar/
        ├── index.html      Palapa Bar menu (mobile-first, responsive)
        ├── qr.html         Printable table-tent with the menu QR code
        └── qr.svg          Standalone QR image (for flyers, coasters, etc.)
```

## Adding another bar

1. Create a new folder `bars/<bar-name>/` and add an `index.html` menu inside it
   (copy `bars/palapa-bar/index.html` as a starting point).
2. Add a card for it on the root `index.html` (copy the Palapa Bar `<a class="bar">`
   block and update the link, emoji, and text).
3. Generate a QR that points to
   `https://javiere66.github.io/sommelierinnovations/bars/<bar-name>/`.

## Notes

- Everything is plain HTML/CSS — no build step. Edit a file, commit, and the live
  site updates automatically once GitHub Pages is enabled.
- Prices are in Mexican pesos (MXN).
