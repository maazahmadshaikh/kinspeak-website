# Kinspeak website

Source for https://kinspeak.ca, served with GitHub Pages.

- `index.html`: the whole site (styles and images are embedded)
- `CNAME`: custom domain for GitHub Pages

## Adding a photo to "Out on the land"

The photos sit in a sliding row (`.slider-track` in `index.html`). To add one,
copy an existing `<figure class="photo slide">…</figure>` line inside that row
and change the image, the `alt` text, the caption and the place:

```html
<figure class="photo slide"><div class="frame"><img src="IMAGE" alt="What the photo shows" loading="lazy"></div><figcaption>Caption<span class="place">Place, NT</span></figcaption></figure>
```

Portrait photos crop best (the frame is 3:4). Keep images under about 300 KB
(WebP, roughly 1000 px tall). The arrows and swiping adjust on their own.
