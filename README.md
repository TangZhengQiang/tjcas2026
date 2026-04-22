# TJCAS 2026 Website

Official static website source for **TJCAS 2026**  
Taiwan and Japan Conference on Circuits and Systems  
August 25-27, 2026, Hamamatsu, Shizuoka, Japan

## Overview

This repository contains the source code and static assets for the TJCAS 2026 conference website.  
The site is implemented as a simple static HTML/CSS project without a build system, which makes it easy to edit, deploy, and maintain.

The website currently includes:

- Home page with conference overview, news, important dates, topics, and past conferences
- Program page
- Organization page
- Submission page
- Registration page
- Contact page
- Venue page
- Custom 404 page

## Project Structure

```text
.
|- index.html
|- program.html
|- organization.html
|- submission.html
|- registration.html
|- contact.html
|- venue.html
|- topics.html
|- 404.html
|- style.css
|- tjcas_Logo.png
|- hamamatsu.jpg
|- venue_reception.png
|- venue_conference.png
|- venue_banquet.png
|- TJCAS2016_CFP.pdf
|- TJCAS2018_CFP.pdf
`- templates/
   |- IEEEtran.zip
   |- sample_1column.docx
   |- sample_1column.tex
   |- sample_2column.docx
   `- sample_2column.tex
```

## Main Files

- `index.html`: Main landing page
- `style.css`: Shared stylesheet for all pages
- `program.html`: Program overview and day-by-day placeholders
- `organization.html`: Organizing committee and steering committee
- `submission.html`: Submission information placeholder
- `registration.html`: Registration information placeholder
- `contact.html`: Secretariat contact page
- `venue.html`: Venue details with maps and official links
- `404.html`: Fallback page for missing routes

## Design and Implementation Notes

- The site uses shared navigation and shared page styling through `style.css`
- No JavaScript is currently required
- Most content is plain HTML for easier manual maintenance
- Responsive behavior is handled with CSS media queries
- External links opened in new tabs use secure `rel="noopener noreferrer"` attributes

## Local Preview

Because this is a static website, you can preview it locally in several simple ways:

1. Open `index.html` directly in a browser.
2. Or run a lightweight local server from the repository root.

Example using Python:

```bash
python -m http.server 8000
```

Then open:

```text
http://localhost:8000/
```

## Content Maintenance

Typical updates for this website include:

- Updating conference dates and news on the homepage
- Replacing `TBA` placeholders in program, submission, and registration pages
- Updating committee information in `organization.html`
- Revising venue details and external links in `venue.html`
- Adding new announcements and links as the conference schedule becomes finalized

## Deployment

This repository is suitable for static hosting platforms such as:

- GitHub Pages
- Netlify
- Vercel static deployment
- Any standard web server serving HTML/CSS/image assets

## Maintenance Suggestions

- Keep shared header/footer content synchronized across pages
- Compress large image assets if page loading speed becomes a concern
- Review all placeholders before public release
- Test both desktop and mobile layouts before publishing major updates

## Repository Purpose

This repository serves as the maintainable source of truth for the TJCAS 2026 website and related static materials.
