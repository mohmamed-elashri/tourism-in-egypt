# Visit Egypt (tourism-in-egypt)

A small static, Arabic (right-to-left) tourism site. It has a home page with a city card and a Cairo page listing three attractions: the pyramids, a museum and a historic market.

No build step and no dependencies: plain HTML and CSS.

## Run locally

Open `index.html` in a browser, or serve the folder:

```
python3 -m http.server 8000
```

then visit http://localhost:8000.

## Structure

```
index.html          home page
cities/cairo.html   Cairo page
styles.css          shared styles
images/             photos
```

## What the design covers

- Responsive grid layout (cards reflow from one column on phones to several on wide screens).
- Right-to-left layout (`dir="rtl"`, logical CSS properties).
- Accessibility basics: landmarks (`header`, `main`, `footer`), skip link, descriptive image alt text, visible keyboard focus, text contrast checked against WCAG AA for the main buttons, reduced-motion respected.
- Light and dark colour schemes via `prefers-color-scheme`.
- Images have explicit dimensions and lazy loading.

## Deployment

The site is published with GitHub Pages from the `main` branch (legacy branch deployment, already enabled): https://mohmamed-elashri.github.io/tourism-in-egypt/ . Changes appear after they are merged into `main`.

## Known gaps

- Only one city (Cairo) exists.
- Photo sources and licences are not recorded in the repository. Add credits before reusing the images publicly.
- Page text is Arabic only.
