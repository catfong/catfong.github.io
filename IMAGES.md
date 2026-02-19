# Images and assets for your site

This file is a short guide so you can add or swap images without touching code.

## Where images go

- Put image files (e.g. `face.jpg`, `forest.jpg`, `hero.jpg`) in the **same folder** as your `.qmd` files (the root of `catfong.github.io/`).
- The site already uses:
  - **face.jpg** — About page and Projects (trait-based seaweed section)
  - **forest.jpg** — Projects (Wildfire in the West)

## Hero image (optional)

To use a **full-width hero image** on the homepage instead of the gradient:

1. Add a file, e.g. `hero.jpg`, to the project root.
2. In `index.qmd`, change the hero block to use it. Replace the opening of the hero div with a version that sets a background image, e.g. in `styles.scss` add:

   ```scss
   .hero-wrap.with-image {
     background-image: linear-gradient(var(--hero-overlay), var(--hero-overlay)), url('hero.jpg');
   }
   ```
   Then add the class `with-image` to the hero div in `index.qmd`.

Or keep the current gradient—it works with no image and stays bold and professional.

## Finding free, professional images

- **Unsplash** (unsplash.com) — Search: "ecology", "coral reef", "forest resilience", "sustainability", "field research", "woman scientist".
- **Pexels** (pexels.com) — Same kinds of terms; good for nature and people.
- **Your own** — Field work, lab, or a clear headshot for `face.jpg` are strongest for a “fund her” vibe.

## Video (optional)

To embed a short video (e.g. 30–60 seconds about your work or a project):

1. Host it on YouTube or Vimeo (unlisted is fine).
2. In any `.qmd` file, add:

   ```markdown
   ::: {.ratio .ratio-16x9}
   <iframe src="YOUR_VIDEO_EMBED_URL" allowfullscreen></iframe>
   :::
   ```

A single, high-impact hero image or one short video on the homepage can make the site feel even more engaging.
