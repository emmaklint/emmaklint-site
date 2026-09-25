# emmaklint.com

Static site, no build step. Everything lives in `index.html` and `styles.css`.

## Deploy on Vercel
1. Push this folder to a new GitHub repo.
2. In Vercel: Add New > Project > import the repo. Framework preset: Other. Leave build settings empty.
3. When it looks right on the preview URL, move the `emmaklint.com` domain from the old project to this one (old project > Settings > Domains > remove, new project > Settings > Domains > add).

## Updating
- Posts: edit the four `<a class="post">` blocks in `index.html`, and drop new images in `/images`.
- Colors: all in the `:root` block at the top of `styles.css`.
