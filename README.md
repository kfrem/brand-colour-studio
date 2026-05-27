# Brand Colour Studio

Static single-page SaaS prototype for `brandcolours.meetingpipeline.com`.

## What It Does

- Builds curated and custom brand colour palettes.
- Extracts colours from uploaded logos locally in the browser.
- Shows website/report previews, WCAG contrast checks and export panels.
- Presents a Pro upgrade flow for PDF, client approval, Tailwind/SCSS and social-card exports.

## Deployment

Host this folder as a static site. The production entry point is `index.html`.

Recommended Hostinger setup:

1. Create the subdomain `brandcolours.meetingpipeline.com`.
2. Connect the subdomain website to this GitHub repository.
3. Use the repository root as the publish directory.
4. Enable automatic deployment on push to `main`.

## Payment Links

Before launch, replace the empty URLs in `CHECKOUT_URLS` inside `index.html` with live Stripe Payment Links or Checkout links:

```js
const CHECKOUT_URLS = {
  monthly: 'https://buy.stripe.com/...',
  lifetime: 'https://buy.stripe.com/...'
};
```

Until those links are configured, upgrade buttons open a pre-filled email request to `hello@meetingpipeline.com` instead of sending users to a broken checkout route.
