A self-contained, mobile-friendly interactive date proposal website. It uses HTML, CSS and vanilla JavaScript; no framework or build step is required.

## Run it locally
1. Extract the ZIP.
2. Open `index.html` in Chrome, Safari or another modern browser.
3. Test the full flow, including the runaway **No** button, date/time selection, food choice, pickup time and joke checkout.

## Publish it
You can upload `index.html` to a static hosting service such as GitHub Pages, Netlify or Replit. No server is required for the basic experience.

## WhatsApp date-plan handoff
The final confirmation screen can prepare a WhatsApp message containing selected date, time, food and ready-by time.

At the top of the `<script>` in `index.html`, find:

```js
const WHATSAPP_NUMBER = "";
```

- Leave it blank to let her choose a WhatsApp chat after the confirmation.
- Or set it to your WhatsApp number with country code and digits only, with no `+`, spaces or punctuation. Example format: `"9715XXXXXXXX"`.

## Important details
- The `$499` checkout is a visual joke only. No payment details are collected and no payment is processed.
- The site does not save choices to a database. The WhatsApp handoff is how the selected plan can be sent to you.
- The selected time is treated as the date time; the website calculates the “be ready by” time exactly one hour earlier.
- Google Fonts are loaded online. If unavailable, the site falls back to system fonts.
