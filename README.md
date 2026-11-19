# Workshop website: Practical Modelling and Simulation of Geothermal Energy Storage

Static one-page site for the open workshop in Oslo, 17–18 March 2027, hosted on GitHub Pages.
No build step: edit the files directly (also works in GitHub's web editor).

| File           | Purpose                                                  |
|----------------|----------------------------------------------------------|
| `index.html`   | All page content                                         |
| `style.css`    | Layout and styling                                       |
| `favicon.svg`  | Browser tab icon                                         |
| `workshop.ics` | "Add to calendar" file                                   |
| `.nojekyll`    | Tells GitHub Pages to serve the files as-is (no Jekyll)  |

## Publish

1. Create the repo under https://github.com/sintefmath and push these files to `main`.
2. In the repo: **Settings → Pages → Build and deployment → Source: Deploy from a branch**,
   branch `main`, folder `/ (root)`.
3. After a minute the site is live at `https://sintefmath.github.io/REPO-NAME/`.

## Before announcing the site

- [ ] Replace `REPO-NAME` in `index.html` (og:url, og:image) and `workshop.ics` (2 places).
- [ ] Insert the registration link in **both** Register buttons (search for `href="#"`).
- [ ] Fill in every yellow placeholder: search `index.html` for `class="ph"` and `ph-block`.
      Remove the `<span class="ph">` wrapper (or the `ph-block` class) once filled.
- [ ] Add `og-image.png` (1200×630 px) for link previews on LinkedIn/Teams/e-mail,
      or remove the `og:image` line.
- [ ] Add the privacy statement link and contact person.
- [ ] Check logo and branding rules before adding logos to the footer.
- [ ] Update the "Last updated" date in the footer whenever you change content.

## When the programme is ready

In `index.html`, the `#programme` section contains a commented-out example table.
Replace the notice paragraph with one `<h3>` + `<table class="programme">` per day.
When start/end times are known, you can also add them to `workshop.ics`, e.g.
`DTSTART;TZID=Europe/Oslo:20270317T090000` and `DTEND;TZID=Europe/Oslo:20270318T160000`.

## Preview locally

Open `index.html` in a browser, or run `python3 -m http.server` in this folder and go to
http://localhost:8000.
