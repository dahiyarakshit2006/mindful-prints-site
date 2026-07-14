# Mindful Prints — single-page website

## Files
- `index.html` — the entire site (inline CSS + vanilla JS, no build step)
- `assets/logo.svg` — primary full-colour lockup
- `assets/logo-black.svg` — single-colour black lockup
- `assets/logo-white.svg` — reversed lockup for dark backgrounds
- `assets/icon-only.svg` — icon mark (favicon / social)
- `assets/icon-white.svg` — icon mark for dark backgrounds
- `sitemap.xml`, `robots.txt` — indexing stubs

## Before you go live — 3 steps

1. **Connect the enquiry form (required — the form does nothing until you do this).**
   - Go to https://web3forms.com and enter `info@mindfulprints.org`. It's free; no account or backend needed.
   - Copy the access key they email you.
   - In `index.html`, find the hidden input `<input type="hidden" name="access_key" value="YOUR_ACCESS_KEY_HERE">` and paste your key into the `value`. (Leave the other two mentions of that placeholder alone — they are a comment and a safety check.)
   - Enquiries will then arrive at info@mindfulprints.org.

2. **Set your real domain.** Search `mindfulprints.org` in `index.html`, `sitemap.xml` and `robots.txt` and replace it if the live domain differs.

3. **Social links.** The three footer icons point to `#`. Swap in the real Instagram (@mindful_printss) and LinkedIn URLs.

## Deploy
- **Netlify / Vercel:** drag this whole folder onto the dashboard. Done, no build command.
- **GitHub Pages:** push the folder to a repo, then Settings → Pages → deploy from `main` / root.

## Post-launch
Submit `https://yourdomain.com/sitemap.xml` in Google Search Console to get indexed.
