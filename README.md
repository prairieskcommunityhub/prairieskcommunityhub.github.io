# Prairie Community & Innovation Hub — Quarto website

A ready-to-customize static Quarto website with colourful clickable homepage cards, pages for community resources and immigration information, and a contact form.

## 1. Install requirements

Install Quarto from https://quarto.org/docs/get-started/ . No R installation is required to render these pages. R is optional for future interactive reports.

## 2. Preview locally

Open this folder in RStudio or a terminal and run:

```sh
quarto preview
```

## 3. Activate the contact form (REQUIRED)

GitHub Pages cannot send emails by itself. This template uses Formspree (https://formspree.io/):

1. Create an account at Formspree, and create a new form.
2. Set your preferred destination email in Formspree and verify it as required.
3. Copy the form endpoint (e.g. `https://formspree.io/f/abcdefgh`).
4. Open `contact.qmd` and replace `YOUR_FORM_ID` with the actual ID (`abcdefgh` in this example).
5. Remove or revise the orange "Setup required" note in `contact.qmd` after you activate the form.
6. Render and publish; submit a test inquiry and confirm receipt in Formspree and your inbox.

**Do not use this form to collect passport details, government identifiers, medical information, or other sensitive information.** Review Formspree's terms, privacy information, spam controls and free plan limits before launching. The form service may process submissions outside Canada.

## 4. Publish to GitHub Pages

This project is configured to generate a `docs/` directory for GitHub Pages branch publishing.

```sh
quarto render
```

Upload the project to the public repository for your GitHub organization, ideally named `prairieskcommunityhub.github.io` (if the organization is `prairieskcommunityhub`). Keep the generated `docs/` directory intact. In the repository settings go to Pages → Deploy from a branch → `main` → `/docs` → Save.

For repeat publishing, use GitHub Desktop to clone the repository, copy the files, commit, and push.

**Important:** If you have an existing Quarto site, back it up first. Either use this as a new project, or merge the files and navbar settings into the existing project. Do not overwrite existing research files or dashboards accidentally.

## 5. Customize

- `_quarto.yml`: site title, domain and navigation.
- `index.qmd`: clickable homepage cards.
- `styles.css`: visual appearance and colours.
- `immigration.qmd`: official Canadian immigration information links.
- `contact.qmd`: form endpoint and privacy notice.
- `research.qmd`, `dashboard.qmd`: add your dashboards and reports.

## Important disclaimers

Immigration-related links are informational, not legal advice. Check IRCC and Saskatchewan official pages for current requirements. This project is an independent community initiative and does not imply government affiliation.
