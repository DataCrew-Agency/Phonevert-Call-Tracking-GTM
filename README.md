# Phonevert-Call-Tracking-GTM

Google Tag Manager **custom tag template** that loads the **Phonevert Call
Tracking** script onto your website.

The tag injects `phonevert.js` from `https://phonevert.ai` and configures it
with your Phonevert API key (`window.phonevertConfig.apiKey`).

## Configuration

- **API Key** – your Phonevert API key (starts with `pk_live_`). As a logged-in
  Phonevert user, copy it from the **Phonevert Base Code** page
  (<https://phonevert.ai/installation>) on the **GTM template** tab.

## ⚠️ Consent

This tag loads a third-party tracking script. It is **important that the tag is
fired in accordance with the visitor's consent** — configure it to respect your
consent management setup (e.g. GTM Consent Mode and/or a consent-gated firing
trigger), so it only runs when the user has granted the relevant consent.

## Setup

1. **Download the template** — Download the `phonevert_call_tracking.tpl` file
   from this repository.

2. **Import into GTM** — In Google Tag Manager go to
   **Templates → Tag Templates → New → ⋮ menu → Import**, then select the
   `.tpl` file.

3. **Create a new tag** — Go to **Tags → New** and choose the Phonevert template
   you just imported.

4. **Enter your API key** — Paste your Phonevert API key into the tag's
   **API Key** field. As a logged-in Phonevert user you can copy it from the
   **Phonevert Base Code** page (<https://phonevert.ai/installation>) on the
   **GTM template** tab.

5. **Set the trigger and consent** — Add the **Initialization — All Pages**
   trigger (or **All Pages**) so it loads on every page. **Important:** Phonevert
   should only run with the appropriate consent.

6. **Save & publish** — Save the tag, then submit and publish your container.
