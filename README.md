# The Cuppa website

Three static pages — home, privacy policy, support — in the app's own look.
No build step. Publish anywhere that serves files; the intended home is a
free GitHub Pages site:

1. Create a **public** repository on GitHub called `cuppa-site` (Pages on a
   free account needs a public repo).
2. Copy the contents of this folder into it and push.
3. Repository → Settings → Pages → Source: *Deploy from a branch*, branch
   `main`, folder `/ (root)`. Save.
4. A minute later the site is at `https://<your-github-username>.github.io/cuppa-site/`.

Before publishing, replace `gaiseranthony@gmail.com` in all three pages with the real
address, and the App Store link in `index.html` once the app is live. Then
put the resulting URLs into App Store Connect (Support URL, Privacy Policy
URL) and into `PRIVACY_URL` in `src/app/paywall.tsx`.
