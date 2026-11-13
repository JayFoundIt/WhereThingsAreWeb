# wherethingsare.at

Placeholder site for Jay: Where Things Are. Plain static files, no build step.

- `index.html` is the whole page; styles and the German/English switch are inline. Nothing is loaded from other hosts.
- `404.html` is what GitHub Pages serves for unknown paths.
- `CNAME` tells GitHub Pages the custom domain. `.nojekyll` switches off Jekyll.
- The icons are scaled from `App/Assets.xcassets/AppIcon.appiconset/icon-1024.png` in the app repository.

Preview locally:

```bash
python3 -m http.server 8765
```

Hosted on GitHub Pages from the `main` branch, root folder.
