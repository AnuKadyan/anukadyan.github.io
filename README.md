# Anu Kadyan: personal website

A plain HTML site with no build step. Each page is one file:

| File | Page |
|---|---|
| `index.html` | Home |
| `research.html` | Research and publications |
| `policy.html` | Policy papers |
| `talks.html` | Writing and talks |
| `archive.html` | Archive of all work, filterable by topic |
| `cv.html` | CV |
| `images/` | Headshot and Loadmatch screenshot |

## Put it online with GitHub Pages

1. Create a free account at github.com. Use your Columbia email so you can claim the Student Developer Pack later.
2. Create a new **public** repository named exactly `YOUR-USERNAME.github.io`.
3. On the repository page, click **Add file → Upload files**. Drag in everything inside this folder, including the `images` folder and the hidden `.nojekyll` file, then click **Commit changes**.
4. Go to **Settings → Pages**. Under "Build and deployment", choose **Deploy from a branch**, then branch `main` and folder `/ (root)`, and click **Save**.
5. After a minute or two the site is live at `https://YOUR-USERNAME.github.io`.

## Add your own domain

1. Buy the domain (see below).
2. In GitHub, go to **Settings → Pages → Custom domain**, enter `yourdomain.com` and save. This creates a `CNAME` file in the repository.
3. At your domain registrar, open the DNS settings and add:
   - Four **A** records for host `@`, pointing to `185.199.108.153`, `185.199.109.153`, `185.199.110.153` and `185.199.111.153`
   - One **CNAME** record for host `www`, pointing to `YOUR-USERNAME.github.io`
4. Wait for DNS to update (from a few minutes up to a day). Then go back to **Settings → Pages** and tick **Enforce HTTPS**.

## Updating the site later

Open a file on GitHub, click the pencil icon, edit the text and commit. The site updates in about a minute.

Placeholders still to fill in: search the files for `[ADD LINK]` (the CV PDF and the paper PDFs) and `[ Image` (the image slots on the home page). To add a PDF, upload it to the repository, for example into a `papers/` folder, and replace `href="#"` with `href="papers/filename.pdf"`.
