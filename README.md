# Zomsi Website

Static company/product website for **zomsi.co**, built with Astro and ready for GitHub Pages.

## Pages

- `/` — Zomsi homepage
- `/apps` — app portfolio
- `/about` — company/about
- `/contact` — contact
- `/rummyscore` — RummyScore marketing page
- `/rummyscore/support` — RummyScore support
- `/rummyscore/privacy` — RummyScore privacy policy

## Run locally

```bash
npm install
npm run dev
```

Production build:

```bash
npm run build
npm run preview
```

## GitHub Pages

1. Create a GitHub repository such as `zomsi-website`.
2. Push this project to `main`.
3. In GitHub open **Settings → Pages**.
4. Set **Source** to **GitHub Actions**.
5. Push to `main`; `.github/workflows/deploy.yml` will deploy the site.
6. `public/CNAME` is already configured for `zomsi.co`.

## DNS for zomsi.co

For the apex domain, add GitHub Pages A records at your registrar:

```text
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```

For `www`, create a CNAME pointing to your GitHub Pages host, for example:

```text
www → YOUR_GITHUB_ORG_OR_USERNAME.github.io
```

Then add `zomsi.co` as the custom domain under **GitHub → Settings → Pages** and enable **Enforce HTTPS** after DNS verification.

## Before launch

Update:

- RummyScore App Store URL in `src/pages/rummyscore/index.astro`
- Google Play URL
- Web app URL
- `support@zomsi.co` if you want a different support/contact email
- Privacy policy wording to exactly match the production app's Firebase/Supabase data practices
- Replace the placeholder RummyScore artwork with your real icon/screenshots when ready

## Company

**Brand:** Zomsi  
**Legal company:** Zomsi Info Tech Private Limited
