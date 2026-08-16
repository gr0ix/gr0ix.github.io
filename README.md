# Security Portfolio (GitHub Pages starter)

A single-page cybersecurity portfolio site, styled like a case file /
incident report. Pure HTML/CSS/JS — no build step, so it works directly
with GitHub Pages.

## 1. Get it on GitHub

```bash
cd cyber-portfolio
git init
git add .
git commit -m "Initial portfolio"
```

Create a new repo on GitHub named `your-username.github.io` (this gives
you a site at the root domain), or any other name (the site will live at
`your-username.github.io/repo-name`).

```bash
git remote add origin https://github.com/your-username/your-repo.git
git branch -M main
git push -u origin main
```

## 2. Turn on GitHub Pages

1. On GitHub, go to your repo → **Settings → Pages**.
2. Under **Build and deployment**, set **Source** to "Deploy from a branch".
3. Set **Branch** to `main` and folder to `/ (root)`.
4. Save. Your site will be live in a minute or two at the URL shown on
   that page.

## 3. Customize the content

Everything is in `index.html` — no templating, just edit the text directly.

- **Your name / title** — hero section near the top.
- **About** (`#about`) — swap in your real bio. The redacted lines
  (black bars that reveal on hover) are a fun detail; keep or remove them.
- **Skills** (`#skills`) — edit the `--w` percentage on each `<i>` bar
  (0–100) to reflect your own self-rated levels.
- **Projects** (`#projects`) — replace the four placeholder "case files"
  with your own repos. Update the `href="#"` links to real GitHub/demo URLs.
- **Writeups** (`#writeups`) — one table row per CTF room/box you've
  written up. Link each to a blog post, a GitHub markdown file, or a
  Medium post.
- **Credentials** (`#credentials`) — your education and certifications.
- **Contact** (`#contact`) — update the email, GitHub, and LinkedIn links.

## 4. Add your resume

Drop a PDF at `assets/resume-placeholder.pdf` (or update the `href` in
the hero's "Download Resume" button to point wherever you keep it).

## 5. Optional: custom domain

If you buy a domain, add a `CNAME` file at the repo root containing just
your domain name, then point your DNS at GitHub's IPs (see GitHub's docs
for "Managing a custom domain for your GitHub Pages site").

## File structure

```
index.html              — all page content, one file
assets/css/style.css    — all styling
assets/js/main.js       — mobile nav toggle + footer year
assets/resume-placeholder.pdf  — add your real resume here
```

## Notes

- No frameworks, no build tools — edit and push, Pages handles the rest.
- Fonts (Space Grotesk, Source Serif 4, JetBrains Mono) load from Google
  Fonts via CDN link tags in `index.html`.
- The design respects `prefers-reduced-motion` and has visible keyboard
  focus states throughout.
