# KREDA Agency Website

Static multilingual landing page for KREDA Agency.

## Files

- `index.html` — main website file
- `assets/kreda-logo.svg` — KREDA logo used in header, footer and favicon
- `vercel.json` — Vercel static deployment config

## Deploy to Vercel

1. Create a new GitHub repository.
2. Upload all files from this folder to the repository root.
3. In Vercel, create a new project from that repository.
4. Use these settings:

```text
Framework Preset: Other
Root Directory: ./
Build Command: leave empty
Output Directory: ./
Install Command: leave empty
```

5. Deploy.

## Local preview

Run from this folder:

```bash
python3 -m http.server 8000
```

Open:

```text
http://127.0.0.1:8000
```

## Notes

- The site supports RU / EN / LV language switching.
- CTA buttons open WhatsApp with prefilled text.
- The form sends the entered data to WhatsApp.
- No build step is required.
