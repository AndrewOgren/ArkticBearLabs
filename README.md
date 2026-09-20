# Arktic Bear Labs — landing page

A static, dependency-free landing page. No build step.

```
index.html    page markup
styles.css    all styling (light + dark, responsive)
favicon.svg   tab icon
```

## Local preview

```sh
python3 -m http.server 8000
# open http://localhost:8000
```

## Deploying

Any static host works — drop the three files at the site root:

- **GitHub Pages:** push to `main`, then Settings → Pages → Deploy from branch → `main` / root.
- **Netlify / Cloudflare Pages / Vercel:** point at this repo, no build command, publish directory `.`.

## Editing

- Copy lives directly in `index.html`; the sections are `#about` and `#contact`.
- Colors are CSS custom properties at the top of `styles.css` (`:root`, plus a
  `prefers-color-scheme: dark` block) — change `--accent` to restyle the whole page.
- Update the contact address (`andrew@arkticbearlabs.com`) in the nav CTA, contact
  section, and footer.
