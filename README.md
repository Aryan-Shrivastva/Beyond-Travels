# Beyond Travels

Beyond Travels is a cinematic, multi-page travel experience for considered journeys across India, Bhutan, Nepal, and China. It uses full-bleed destination imagery, route cards, package details, country and terrain filters, and CSS-driven layouts to help visitors move from inspiration to a specific trip.

## Pages

- `index.html` — cinematic home page and journey discovery panels
- `destinations.html` — country and terrain selector
- `packages.html` — package collections and combined filters
- `package.html` — hash-addressable package detail articles
- `about.html` — story, values, and responsible travel notes
- `contact.html` — enquiry form and FAQ
- `404.html` — lost-route page

## Run locally

This is a static HTML and CSS site. No framework, JavaScript runtime, package install, or build step is required.

1. Open `index.html` directly in a browser, or serve the folder with any static file server.
2. For example, with Python installed:

   ```text
   python -m http.server 8000
   ```

3. Visit `http://localhost:8000/`.

Serving the folder is recommended because relative image paths and hash links behave consistently over HTTP.

## Project structure

All shared styling lives in `style.css`. Destination and package photography is stored in `images/`. The site uses native HTML controls, radio selections, `:has()`, `:target`, and `prefers-reduced-motion` rules for its interactive states.

The enquiry form is currently a front-end form only. Its submit action is intentionally disabled until a real form endpoint or backend is connected.

## Adding images

Keep new images in `images/`, use descriptive filenames, and add meaningful `alt`, `width`, and `height` attributes to every new `<img>`. Existing CSS gradients provide a dark fallback behind image areas when an asset is unavailable.
