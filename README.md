# Phonevert-Call-Tracking-GTM

Google Tag Manager **custom tag template** that loads the **Phonevert Call
Tracking** script onto your website.

The tag injects `phonevert.js` from `https://phonevert.ai` and configures it
with your Phonevert API key (`window.phonevertConfig.apiKey`).

## Configuration

- **API Key** – your Phonevert API key (starts with `pk_live_`), found on the
  Installation page of your Phonevert dashboard.

## ⚠️ Consent

This tag loads a third-party tracking script. It is **important that the tag is
fired in accordance with the visitor's consent** — configure it to respect your
consent management setup (e.g. GTM Consent Mode and/or a consent-gated firing
trigger), so it only runs when the user has granted the relevant consent.

## Installation

1. In GTM, go to **Templates → Tag Templates → New** and import
   `phonevert_call_tracking.tpl`.
2. Create a new tag from the template and set the **API Key**.
3. Add a firing trigger that is **gated by consent**.
