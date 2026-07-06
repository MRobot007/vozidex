# VOZIDEX

A single-file marketing site for **VOZIDEX** — a Rajkot-based dealer for buying, renting, and accessorising performance & luxury cars.

## Highlights

- **One self-contained file** (`index.html`) — all HTML, CSS, and JS inline. No build step, no framework.
- **Glassmorphism** dark UI with an electric-red performance theme and a blurred brand-logo backdrop.
- **Hero** — bleeding-car feature cards (Buy / Rent) over frosted glass.
- **Live stock grid** with client-side search, filter pills (Sale / Rent / Accessories), "popular makes" and body-type filters, and a favourites system (persisted to `localStorage`).
- **Enquiry form** that emails submissions via [formsubmit.co](https://formsubmit.co) (no backend required).
- Animated effects powered by **anime.js** (`assets/anime.min.js`), with full `prefers-reduced-motion` support.
- Responsive down to 375px, semantic HTML, skip link, ARIA labels, and a `LocalBusiness` JSON-LD block.

## Run locally

It's a static file — open `index.html` directly, or serve the folder:

```bash
# any static server, e.g.
npx serve .
# then visit http://localhost:3000
```

## Configuration

Edit the `CONFIG` block near the top of the `<script>` in `index.html`:

```js
const CONFIG = {
  enquiryEmail: "mihir.r.bhavsar1336@gmail.com" // where enquiry-form submissions are emailed
};
```

> The first form submission triggers a one-time **formsubmit.co activation email** to that address — click "Activate" once and enquiries flow automatically after that.

## Structure

```
index.html            # the entire site
assets/
  ├─ *.png            # transparent car cut-outs + logo
  └─ anime.min.js     # animation library (MIT, bundled locally)
```
