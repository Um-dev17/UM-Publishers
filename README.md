# UM Publishers Website

A responsive, ten-page publishing-agency concept built for a Web Engineering university assignment.

## Technologies
- HTML5 semantic markup
- CSS3 (Grid, Flexbox, media queries, transitions, keyframes)
- Original local SVG artwork for book covers, brand icon, and hero illustration
- No JavaScript, framework, backend, database, or external image dependency

## Pages
1. `index.html` — Home
2. `about.html` — About Us
3. `services.html` — Services
4. `publishing.html` — Book Publishing
5. `marketing.html` — Book Marketing
6. `portfolio.html` — Our Books / Portfolio
7. `packages.html` — Packages
8. `process.html` — Our Process
9. `faq.html` — Frequently Asked Questions
10. `contact.html` — Contact and demonstration enquiry form

## Project structure
```text
UM-Publishers-Website/
├── index.html
├── about.html
├── services.html
├── publishing.html
├── marketing.html
├── portfolio.html
├── packages.html
├── process.html
├── faq.html
├── contact.html
├── css/
│   └── style.css
├── assets/
│   └── images/
│       ├── favicon.svg
│       ├── publishing-hero.svg
│       └── [10 original sample book cover SVGs]
├── README.md
└── ARCHITECTURE.md
```

## Run locally
1. Download and extract the ZIP.
2. Open `index.html` in a modern browser.
3. Use the navigation to visit the other pages. No build step or server is required.

## Upload to GitHub
1. Create a new repository on GitHub.
2. Extract this ZIP and open the project folder.
3. Upload the contents of `UM-Publishers-Website` (the HTML files, `css`, `assets`, and documentation) to the repository root.
4. Commit the files. The repository should show `index.html` at its root.

Alternatively, from a terminal in the project folder:
```bash
git init
git add .
git commit -m "Add UM Publishers website"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git
git push -u origin main
```
Replace the example remote with your own repository URL.

## Deploy on GitHub Pages
1. Push the project to GitHub with `index.html` in the repository root.
2. Open **Settings → Pages** in the repository.
3. Under the build/deployment settings, choose **Deploy from a branch**.
4. Select the `main` branch and `/ (root)` folder, then save.
5. Wait for the published URL to appear. This is a static site, so no build command is needed.

## Deploy on Netlify
1. Sign in to Netlify and choose **Add new site / Import an existing project**.
2. Connect the GitHub repository, or drag and drop the extracted project folder into Netlify's manual deploy area.
3. Use no build command and leave the publish directory as the project root (where `index.html` lives).
4. Deploy. The site uses relative local paths and does not require environment variables.

## Important limitations
- The contact form is for demonstration only. It has no backend and does not transmit or save information. Do not enter private details.
- All sample book titles, package prices, testimonials, and contact details are illustrative assignment content.
- The project does not claim verified business credentials or guarantee retailer acceptance, sales, reviews, or marketing results.
