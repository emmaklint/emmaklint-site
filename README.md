# emmaklint.com

Static site, no build step. Pages are `index.html` (home), `portfolio.html` (`/portfolio`), `services.html` (`/services`) and one page per project in `work/` (e.g. `work/ai-is-a-spectrum.html` at `/work/ai-is-a-spectrum`), all sharing `styles.css`. The header and footer are copied into each page, so edit all of them when changing them.

## Deploy on Vercel
1. Push this folder to a new GitHub repo.
2. In Vercel: Add New > Project > import the repo. Framework preset: Other. Leave build settings empty.
3. When it looks right on the preview URL, move the `emmaklint.com` domain from the old project to this one (old project > Settings > Domains > remove, new project > Settings > Domains > add).

## Updating
- Posts: edit the four `<a class="post">` blocks in the Writing section of `index.html`, and drop new images in `/images`.
- Projects: each project is an `<article class="project">` row (screenshot left, text right). Add a new one above the others in `portfolio.html`, and in the "Things I’m exploring" section of `index.html` if it belongs there. For a project page, copy `work/ai-is-a-spectrum.html` (its sections are `.case-section` text blocks and `.case-gallery` screenshot blocks), put images in `/images/<project>/`, and add the URL to `sitemap.xml`.
- Colors: all in the `:root` block at the top of `styles.css`.
