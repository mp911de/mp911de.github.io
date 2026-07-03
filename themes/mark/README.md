# mark

A quiet, zen Hugo theme. Made for tired minds and eyes.

- Warm light palette (`#493232` on `#fffaf3`), warm dark variant
- Follows the system color scheme with zero JavaScript; one ~20-line inline
  script powers the moon switcher (localStorage override, dusk cross-fade)
- Vanilla CSS, no framework, no build step
- Server-side code highlighting via asciidoctor + rouge (no highlight.js)
- Inline Font Awesome social icons with a gentle celestial hover glow
- No hamburger menu, no pagination, no analytics, no CDNs

## Config

```toml
theme = 'mark'

[params]
  color = 'warm'            # warm (default), linen, gray, light
  name = 'Mark Paluch'      # header brand, falls back to site title
  github = 'mp911de'
  bluesky = 'mp911.de'
  rss = true
  # twitter, instagram, linkedin, mastodon, threads also supported
  mainSections = ['post']
  favicon = 'favicon.ico'
  faviconSvg = 'favicon.svg'
  appleTouchIcon = 'apple-touch-icon.png'

[menu]
  [[menu.main]]
    name = 'About'
    url = '/about/'
    weight = 10

[markup.asciidocExt.attributes]
  source-highlighter = 'rouge'
```

The home page lists the 15 most recent posts grouped by year, followed by a
link to `/archive/`. Create `content/archive.md` with `layout = 'archive'` to
render the full year-grouped archive.

## License

Apache-2.0. Social icons from [Font Awesome Free](https://fontawesome.com)
(CC BY 4.0).
