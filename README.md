# Portfolio Website

A single-page portfolio site — no build step, no dependencies beyond Google Fonts.

## Files
- `index.html` — the whole site (HTML + CSS + JS in one file)
- `assets/photo.jpg` — profile photo
- `assets/resume.pdf` — downloadable résumé, linked from the nav and contact section

## Host it for free on GitHub Pages

1. **Create a new repo** on GitHub. Name it either:
   - `dharun15.github.io` (username-based — this gives you `https://dharun15.github.io/` as the URL), or
   - anything else, e.g. `portfolio` (gives you `https://dharun15.github.io/portfolio/`)

2. **Upload the files** — either:
   - Drag `index.html` and the `assets` folder into the GitHub web UI ("Add file" → "Upload files"), or
   - From your terminal:
     ```
     git clone https://github.com/Dharun15/<repo-name>.git
     cd <repo-name>
     cp /path/to/index.html .
     cp -r /path/to/assets .
     git add .
     git commit -m "Add portfolio site"
     git push
     ```

3. **Turn on GitHub Pages**:
   - Go to your repo → **Settings** → **Pages** (left sidebar)
   - Under "Build and deployment", set **Source** to `Deploy from a branch`
   - Set **Branch** to `main` and folder to `/ (root)`
   - Click **Save**

4. Wait 1–2 minutes, then visit the URL GitHub shows you on that same Pages settings screen.

## Updating later
Edit `index.html` directly (it's plain HTML/CSS/JS — search for the section you want, e.g. `id="experience"`), commit, and push. Changes usually go live within a minute.

## Notes
- Phone number was left off the public site intentionally — email/LinkedIn/GitHub are enough for outreach; add it back in the `hero-links` or `contact` section if you want it.
- To swap the photo, just replace `assets/photo.jpg` with a new file of the same name. Same for `assets/resume.pdf` when you update your résumé — the filename stays the same so the download links keep working.
- Project cards don't link to individual GitHub repos because I don't have real repo URLs for each one — only your GitHub profile as a whole. If you push individual project repos, add a `card-link` (see the Mini-vLLM card's HTML for the pattern) pointing at the real URL instead of the "see GitHub profile" placeholder text.
- Two research items ("Weakly Supervised Video Anomaly Detection" and "Smart Waste Segregation System") show a status line instead of a link since they're under review / recently accepted with no public DOI yet — swap in a real link once one exists.
- Left off: high school grade/percentage and spoken languages (Tamil, Hindi, Malayalam, English/IELTS) from the older CV — lower-signal for a US tech-recruiting audience. Easy to add back under Education if you want them.
