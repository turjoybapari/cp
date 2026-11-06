# CP Solve Hub — publish it as a link (free, ~2 minutes)

`index.html` is the whole app in one file. No server, no database, no build step.
Each visitor's ticks, notes and CP-31 handle are stored in **their own browser**
(localStorage), so nothing is ever uploaded and nobody can see anyone else's progress.

---

## Option A — Netlify Drop (fastest, drag & drop)

1. Go to **https://app.netlify.com/drop**
2. Drag the **folder** `share-cp-hub` (or the zip) onto the page.
3. You instantly get a URL like `https://random-name-123.netlify.app`.
   **No account is needed to drop.** But an unclaimed drop sits behind a temporary
   password and expires — so do the next step.
4. Click **Claim this site** and sign up free (Google/GitHub login works). Now the
   link is public and permanent. Site configuration → Change site name gives you
   something clean like `https://cp-solve-hub.netlify.app`.
5. Send that link to your teammates. Done.

Netlify's free plan is 300 credits/month, which is far more than a single HTML page
needs. To publish an updated version later, drag the folder again onto the site's
**Deploys** page — the URL does not change.

## Option B — Cloudflare Pages (fastest global CDN, free forever)

1. **https://dash.cloudflare.com** → Workers & Pages → Create → Pages → Upload assets
2. Name it `cp-solve-hub`, upload the folder, Deploy.
3. URL: `https://cp-solve-hub.pages.dev`

## Option C — GitHub Pages (best if you already use GitHub)

1. Create a public repo, e.g. `cp-solve-hub`.
2. Upload `index.html` to the root.
3. Settings → Pages → Source: Deploy from a branch → Branch: `main` / `root` → Save.
4. URL: `https://<your-username>.github.io/cp-solve-hub/`
5. To update later, just replace `index.html` — the link stays the same.

## Option D — GitHub Gist trick (no repo needed)

1. **https://gist.github.com** → paste the contents of `index.html`, filename `index.html` → Create public gist.
2. Open `https://htmlpreview.github.io/?<gist-raw-url>` — instant rendered page.
   (Slower and less reliable than A/B/C; use only for a quick demo.)

---

## Important warnings

- **Google Drive will NOT render this HTML.** Drive stopped serving web pages in 2019.
  If you put it on Drive, teammates can only download it, not open it as a page.
- **Do not rename it to `.txt`.** Keep `index.html`.
- **Updating:** re-upload the same `index.html` filename. Everyone's saved progress
  survives, because progress lives in the browser, not in the file.
- **Privacy:** the file contains zero personal data. Verified — a fresh browser
  opens with empty ticks, empty notes and an empty CP-31 handle.

## If you host it, tell your team this

> Open the link on your own phone/laptop. Tick contests and write notes as you go —
> it saves automatically in YOUR browser only. Nobody else can see your progress.
> Don't clear your browser data or you'll lose your ticks. Use My List → Backup to
> save a copy of your progress, and Restore to load it on another device.
