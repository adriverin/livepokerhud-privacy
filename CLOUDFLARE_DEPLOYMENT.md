# Cloudflare Pages Deployment

This repository is ready to deploy as a static Cloudflare Pages project.

## Pages Setup

1. In Cloudflare, open **Workers & Pages**.
2. Create a new **Pages** application.
3. Import the GitHub repository `adriverin/livepokerhud-privacy`.
4. Use these build settings:
   - Production branch: `main`
   - Build command: leave blank, or use `exit 0`
   - Build output directory: `/`
5. Deploy the project.

## Custom Domain

After the first Pages deployment is live:

1. Open the Pages project.
2. Go to **Custom domains**.
3. Add `livepokerhud.com`.
4. Add `www.livepokerhud.com` if you want the `www` host to work.
5. Keep `livepokerhud.com` as the canonical domain. The repository includes a `_redirects` rule that redirects `www.livepokerhud.com` to `livepokerhud.com`.

## App Store URLs

Use these URLs in App Store Connect:

- Privacy Policy: `https://livepokerhud.com/#privacy`
- Terms of Use: `https://livepokerhud.com/#terms`
- Support: `https://livepokerhud.com/#support`

The standalone terms page remains available at:

- `https://livepokerhud.com/terms-of-use.html`
