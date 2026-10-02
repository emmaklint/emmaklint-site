# emmaklint.com

Static site, no build step. Pages are `index.html` (home), `portfolio.html` (`/portfolio`) and `services.html` (`/services`), sharing `styles.css`. The header and footer are copied into each page, so edit all three when changing them.

## Deploy on Vercel
1. Push this folder to a new GitHub repo.
2. In Vercel: Add New > Project > import the repo. Framework preset: Other. Leave build settings empty.
3. When it looks right on the preview URL, move the `emmaklint.com` domain from the old project to this one (old project > Settings > Domains > remove, new project > Settings > Domains > add).

## Updating
- Posts: edit the four `<a class="post">` blocks in the Writing section of `index.html`, and drop new images in `/images`.
- Projects: replace the placeholder `<article class="post">` cards in `portfolio.html` and the Selected work section of `index.html`. Swap the colored `<div class="project-image">` for an `<img>` (or wrap the card in `<a class="post">` to link it). Remove the `noindex` line in `portfolio.html` and add `/portfolio` to `sitemap.xml` once real projects are in.
- Colors: all in the `:root` block at the top of `styles.css`.
