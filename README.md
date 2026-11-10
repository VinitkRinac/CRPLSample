# Rinac Constructor website

Static site (HTML/CSS/JS, no build step).

## Structure
```
index.html, about.html, team.html, solutions.html, layout.html, contact.html, 404.html
assets/css/style.css
assets/js/main.js
assets/img/*.svg
sitemap.xml, robots.txt, .nojekyll
.github/workflows/pages.yml
```

## Deploy on GitHub Pages
1. Create a repo and push everything in this folder to the `main` branch (files must be at the repo root).
2. In the repo go to **Settings → Pages → Build and deployment → Source: GitHub Actions**.
3. Push (or run the workflow from the **Actions** tab). The site goes live at
   `https://<username>.github.io/<repo>/`.

The workflow automatically replaces `https://www.example.com` in `sitemap.xml` and `robots.txt`
with your live URL. If you later add a custom domain, change those two files to your domain and
add a `CNAME` file containing it.

## Before going live
1. Replace `info@rinac.example` and `+91 00000 00000` in the HTML files and in `assets/js/main.js` (`SITE`).
2. The enquiry form opens the visitor's email app (mailto). For a server-side form, point it to a form service.
3. Review the team names and descriptions in `assets/js/main.js` (currently placeholders).
4. Add your office address in `contact.html`.
