# kormoranlabs-website

The one-page site for [kormoranlabs.com](https://www.kormoranlabs.com): Kormoran Labs and its two
products, [Minute Studio](https://minute-studio.com) and Reverun.

Plain static files, no build step. `index.html` is the page, `assets/site.css` the styles of every page,
`reverun/privacy/` the Reverun privacy policy (the URL for the App Store and Google Play). GitHub Pages serves
the repository root (`CNAME`).

- `favicon.svg`, `favicon.ico`, `apple-touch-icon-180.png`: tab and home-screen icons.
- `assets/brand/`: the logo pack v1 (marks, lockups, colours and rules in `README.txt`).
- `assets/minute-studio.png`, `assets/reverun.png`: the products' app icons.
- `assets/og.png`: the link preview image.
- `assets/fonts/`: the three typefaces, self-hosted.
- `assets/screens/`: product screens (WebP, 2x phone size), captured from the Minute Studio and Reverun builds.

Type and colour follow the logo pack: Syne Bold for KORMORAN, Cormorant Garamond for text,
JetBrains Mono for labels, served from `assets/fonts/` (Latin subset, SIL OFL) so no visitor data goes to Google; Abyss ground, Moonbone text, the emerald eye as the only
accent. The page follows the system's light or dark setting. Preview it by opening `index.html`
or with `python3 -m http.server`.
