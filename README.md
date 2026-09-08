# Nikolina Đurović — gestalt psychotherapy

Static one-page site. Structure:

```
index.html      — the whole page
styles.css      — styles (Classical design system)
images/         — hero.png, gestalt.webp, portret.webp
.nojekyll       — required! without it GitHub changes how the site looks
```

**Important:** all four items must be in the repository, including the hidden `.nojekyll` file.
If `styles.css` is not uploaded or `.nojekyll` is left out, the site on GitHub will look
different — no colors, different fonts and layout.

## Hosting on GitHub Pages

1. Create a repository on GitHub (e.g. `nikolina-djurovic`).
2. Put everything from this folder in the repository root (`index.html`, `styles.css`, `images/`).
3. Settings → Pages → Source: `Deploy from a branch`, Branch: `main`, folder: `/ (root)`.
4. The site will be at `https://<username>.github.io/<repo>/`.

For a custom domain: Settings → Pages → Custom domain, then add a CNAME record at your registrar pointing to `<username>.github.io`.

## Replacing images

Replace the files in `images/` using the same names and everything works with no code changes:
- `hero.png` — horizontal, ~2400 × 1000 px, subject on the right
- `gestalt.webp` — vertical 4:5, min. 1200 × 1500 px
- `portret.webp` — vertical 4:5, min. 1200 × 1500 px

## Contact form

Right now it only shows a confirmation — it does not send email. The easiest way to really send is Formspree:
create a form at formspree.io and in `index.html` add `action="https://formspree.io/f/YOUR-ID" method="POST"`
to `<form id="kontakt-forma">`, then delete the `<script>` block at the bottom.

## Check before publishing

- The crisis line number in the footer.
- Education, supervision, address, email and phone details.
- Client testimonials are examples — publish only with written consent.

## Mobile version

The site is responsive within the same `index.html` — there is no separate mobile page. Up to 768px wide: burger menu, hero without the image, all columns in a single stack, the pricing table as cards, full-width form.
