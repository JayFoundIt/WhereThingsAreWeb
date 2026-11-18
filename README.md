# wherethingsare.at

Home page for Jay: Where Things Are and its sister app Wren. Plain static files, no build step.

- `index.html` is the home page: Jay (blue) and Wren (green) side by side, stacked on phones. Styles
  and the German/English switch are inline. Nothing is loaded from other hosts.
- `privacy.html` and `imprint.html` (Datenschutz, Impressum) hold both languages; a German browser
  gets German, the links at the top switch. They share `legal.css`.
- `downloads/Wren-<version>.zip` is the notarized Mac build of Wren, zipped with
  `ditto -c -k --sequesterRsrc --keepParent Wren.app Wren-<version>.zip` (keeps the signature and the
  stapled ticket). For a new version, add the new zip and change the link and the size on the page.
- Jay's beta is on TestFlight: https://testflight.apple.com/join/M3QuCw3m
- `404.html` is what GitHub Pages serves for unknown paths.
- `CNAME` tells GitHub Pages the custom domain. `.nojekyll` switches off Jekyll.
- Jay's icons are scaled from `App/Assets.xcassets/AppIcon.appiconset/icon-1024.png` in its
  repository, `wren-512.png` from Wren's `Apps/iOS/Assets.xcassets/AppIcon.appiconset/icon-1024.png`.

Preview locally:

```bash
python3 -m http.server 8765
```

Hosted on GitHub Pages from the `main` branch, root folder.
