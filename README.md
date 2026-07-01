# Static Academic Homepage Template

This repository contains a static academic homepage template for a GitHub Pages user site.

The visual style is inspired by the compact academic homepage style popularized by [jonbarron/jonbarron.github.io](https://github.com/jonbarron/jonbarron.github.io).

## Quick Start

Open `index.html` directly in a browser, or publish the repository through GitHub Pages.

If you want a local HTTP preview, run:

```bash
python3 -m http.server 4000
```

Then open:

```text
http://localhost:4000
```

## Files And Folders

| Path | Purpose |
| --- | --- |
| `index.html` | Main homepage. Edit this for profile text, news, publications, and projects. |
| `stylesheet.css` | All visual styling. Edit this for fonts, spacing, colors, and responsive layout. |
| `assets/favicon/` | Browser tab icons, using Jon Barron's favicon files while keeping repository root clean. |
| `assets/img/` | Avatar, publication thumbnails, project images, and other images. |
| `assets/pdfs/` | CV, papers, posters, slides, and other downloadable PDFs. |

## Updating Your Profile

In `index.html`, replace:

- `Your Name`
- `Your Role / Affiliation`
- the biography paragraphs
- the links in the `<p class="links">` block
- `assets/img/avatar-placeholder.svg` with your own portrait path

Put your CV at `assets/pdfs/cv.pdf`, or update the CV link to the correct filename.

## Changing The Profile Photo Shape

The profile image uses `profile-photo` plus one shape class in `index.html`:

```html
<img class="profile-photo photo-square hoverZoomLink" ...>
```

Use one of these shape classes:

- `photo-square`: keeps the original image ratio and uses square corners.
- `photo-rounded`: keeps the original image ratio with lightly rounded corners.
- `photo-circle`: crops to a circle, matching the Jon Barron style.

## Images And PDFs

- Store images in `assets/img/`.
- Store downloadable files in `assets/pdfs/`.
- Prefer small optimized thumbnails for publication and project images.

## Styling

Edit `stylesheet.css` to change typography, spacing, colors, or responsive behavior. The main reusable classes are:

- `.profile-table` for the intro area.
- `.news-table` for updates.
- `.experience-table` for education and experience rows.
- `.entry` for publication and project rows.
- `.links` for compact link lists.
