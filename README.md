# ivansadovyi.github.io

Website of Ivan Sadovyi's Wear OS watch faces: catalogue, support and privacy policy.
Plain static HTML and CSS served by GitHub Pages: no build step, no JavaScript, no cookies,
no third-party requests.

| Path | Page |
|---|---|
| `/` | Home and watch face catalogue |
| `/support/` | FAQ and contact |
| `/privacy/` | Privacy policy, linked from every Play listing |

## When a watch face goes live on Google Play

In `index.html`, each card carries its package in `data-package`. Replace the card's

```html
<div class="face__store"><span class="store-link store-link--soon">Google Play</span><span class="chip">COMING SOON</span></div>
```

with

```html
<div class="face__store"><a class="store-link" href="https://play.google.com/store/apps/details?id=PACKAGE">Google Play ↗</a></div>
```

## Notes

- Face images in `assets/faces/` are the store previews (`<face>/store/preview.png` in the
  watch face project), converted to WebP.
- If the privacy policy changes, update its "Last updated" date and `sitemap.xml`.
- Search Console verification files (`google*.html`) live in the root and must not be removed.
