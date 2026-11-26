# kormoranlabs-website

The one-page site for [kormoranlabs.com](https://www.kormoranlabs.com): Kormoran Labs and its two
products, [Minute Studio](https://minute-studio.com) and Reverun.

Plain static files, no build step. `index.html` is the page, `assets/site.css` the styles of every page,
`reverun/privacy/` and `reverun/support/` the Reverun privacy policy and support page (the URLs for the App Store and Google Play), `legal/` the legal notice (mentions légales; linked from every footer). `blog/` the blog: `blog/index.html` lists the posts, each post is a folder with an `index.html`, `blog/feed.xml` is the Atom feed. GitHub Pages serves
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

## Writing a blog post

1. Copy `blog/you-are-not-a-goldfish/` to `blog/<short-slug>/` and edit its `index.html`: title,
   description, canonical and `og:` URLs, the date (both the `datetime` attribute and the text), the
   summary and the text. Replace or delete the copied images (`*.webp`, and `og.jpg`, the 1200 x 630
   link preview).
2. Add the post at the top of the list in `blog/index.html`.
3. Add an `<entry>` at the top of `blog/feed.xml` and set the feed's `<updated>` to the new date.
