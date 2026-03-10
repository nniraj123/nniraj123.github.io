# Niraj Agarwal — Personal Portfolio Webpage

My personal academic portfolio (https://yourusername.github.io)
Current Position: Research Scientist II at [CIRES](https://cires.colorado.edu), embedded within [NOAA's Physical Sciences Laboratory](https://psl.noaa.gov) at the University of Colorado Boulder.

Live site: **https://yourusername.github.io**

---

## About

This is a single-page static website built with plain HTML, CSS, and JavaScript — no frameworks, no build tools, no dependencies beyond Google Fonts. It covers:

- Research overview and biography
- Research interests and focus areas
- Peer-reviewed publications with DOI links
- Research positions and experience
- Selected talks and presentations
- Technical skills
- Contact form and details

## Structure

```
.
├── index.html   # Entire site — HTML, CSS, and JS in one file
└── README.md
```

---

## Updating the Site

All content lives in `index.html`. Each section is marked with a comment like `<!-- PUBLICATIONS -->`, `<!-- TALKS -->`, etc. Use your editor's find (`Ctrl+F` / `Cmd+F`) to jump to the right section quickly.

**Adding a publication** — find `<!-- PUBLICATIONS -->` and copy an existing `.pub-item` block. Update the year, title, authors, journal, DOI link, and badge. Available badge classes: `badge-grl`, `badge-james`, `badge-jfm`, `badge-ocean`, `badge-spotlight`.

**Adding a talk** — find `<!-- TALKS -->` and copy an existing `.talk-item` block. Update the year, title, venue, and type (Oral / Poster / Invited).

**Adding a position** — find `<!-- EXPERIENCE -->` and copy an existing `.exp-item` block. Update the period, organisation, location, role, and description.

**Adding a research interest** — find `<!-- RESEARCH INTERESTS -->` and copy an existing `.interest-card` block. Update the icon, title, and description.

**Adding a skill** — find `<!-- SKILLS -->` and add a `<span class="skill-tag">New Skill</span>` inside the relevant group, or copy a full group block to add a new category.

**Updating contact details or the profile card** — find `<!-- HERO -->` and edit the `.info-row` entries directly.

**Wiring up the contact form** — the form currently has a frontend-only stub. To make it functional, replace the `handleSubmit` function with a `fetch` POST to a service like [Formspree](https://formspree.io).

After any edit:

```bash
git add index.html
git commit -m "your message"
git push
```

GitHub Pages typically rebuilds within 1–2 minutes. Hard refresh (`Cmd+Shift+R` / `Ctrl+Shift+R`) if the old version still shows.

---

## Hosting

Hosted via [GitHub Pages](https://pages.github.com) — free, no server required. The `main` branch root is the deployment source.

---

## Contact

**Niraj Agarwal**  
CIRES / NOAA Physical Sciences Laboratory  
University of Colorado Boulder  
325 Broadway, Boulder, CO 80305  
niraj.agarwal@colorado.edu
