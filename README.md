# [shah20.github.io](https://shah20.github.io)

Personal portfolio of **Rushabh Shah**, Senior Software Engineer. It covers selected work, professional experience, skills, AWS certifications (verifiable on Credly), and contact details.

Live site: **https://shah20.github.io**

## Tech

- Static HTML and CSS with no build step, frameworks, or JavaScript
- Hosted on GitHub Pages
- Light and dark themes that follow the visitor's system preference
- Responsive layout for mobile, tablet, and desktop

## Structure

```
.
├── index.html                    # Portfolio homepage (markup + SVG icon sprite)
├── 404.html                      # Custom "page not found" page
├── assets/
│   ├── style.css                 # Shared styles for all pages
│   ├── photo.jpg                 # Profile photo (480×480, optimised)
│   ├── og-image.jpg              # 1200×630 link-preview card
│   └── Rushabh_Shah_Resume.pdf   # Resume linked from the site
└── _config.yml                   # GitHub Pages / Jekyll config
```

## Run locally

```sh
python3 -m http.server 8000
```

Then open http://localhost:8000.

## Updating content

- **Site content:** edit [index.html](index.html). Each section (`#about`, `#work`, `#experience`, `#skills`, `#credentials`, `#contact`) is clearly marked.
- **Resume:** replace `assets/Rushabh_Shah_Resume.pdf` and keep the same file name so existing links continue to work. The LaTeX source is maintained separately in Overleaf.
- **Theme colours:** adjust the CSS variables in `:root` (light) and the `prefers-color-scheme: dark` block at the top of [assets/style.css](assets/style.css).
- **Icons:** defined once as `<symbol>`s at the top of `index.html` and reused with `<svg class="ico"><use href="#i-name" /></svg>`.

## Deployment

Pushing to the default branch publishes the site automatically through GitHub Pages.
