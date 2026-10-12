# Beyond Borders Outsourcing website

Single-page marketing site for Beyond Borders Outsourcing Services Inc.

## Contents

- `index.html`: the whole site in one self-contained file (styles, scripts and logo are inline). The only external request is Google Fonts.
- `assets/logo/`: the infinity logo as SVG, with PNG copies in `assets/logo/png/`.

## Running it

Open `index.html` in a browser, or serve the folder with any static host (Cloudflare Pages, Vercel, Netlify, GitHub Pages).

## Consultation form

The form sends a JSON `POST` to `/api/consultation` with the fields `name`, `company`, `email`, `phone`, `service`, `size` and `message`. That endpoint is not part of this repository, so on a plain static host the form shows its "not sent" message with the email and phone fallback. Add a serverless function at that path, or point the form at a form service, before going live.
