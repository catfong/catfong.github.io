# Visual assets for your site

Drop your own images and video here so the site can use them directly. Once files are in place, we can point the homepage and other pages to these paths.

## Suggested files

| File | Used for | Notes |
|------|----------|--------|
| **images/hero.jpg** (or .png) | Homepage hero background (fallback when video doesn’t load), and inner-page banners | High-res, landscape; e.g. 1920×1080 or larger |
| **video/hero.mp4** | Homepage hero background video | e.g. download from [Pexels](https://www.pexels.com/video/1448735/) and save here |
| **images/face.jpg** | About page profile photo | Square or portrait; will be shown as a circle |
| **images/banner.jpg** | Optional: different banner for About / Projects / Publications | Same specs as hero if you want variety |

## Paths the site will use

- **Hero image:** `assets/images/hero.jpg` — homepage hero fallback + inner-page banners.
- **Hero video:** `assets/video/hero.mp4` — homepage hero background (optional).
- **About photo:** keep `face.jpg` in `docs/` or add `assets/images/face.jpg` and we'll point About to it.

If a file is missing, the site falls back to the current placeholder (e.g. Unsplash). Add or replace files anytime; we can update the HTML to use `assets/...` once you’re happy with the assets.
