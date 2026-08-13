# Endless Styles Fest Migration Notes

Read-only rescue copy captured from `https://endlessstyles.org/`.

## Safety Rules

- Do not delete, unpublish, or modify the current Replit app while this is being verified.
- Do not change DNS until Hermes confirms the Vercel preview works.
- Do not deploy from this package until the external dependencies below are confirmed.

## Captured

- Single-page React/Vite app: `index.html`
- JavaScript and CSS bundle under `assets/`
- Root image/logo assets
- Sponsor logo assets under `logos/`
- Photo gallery assets under `photos/`
- `favicon.svg`

## External Dependencies To Keep Alive

- Google Fonts: `fonts.googleapis.com`, `fonts.gstatic.com`
- YouTube embed is referenced by the app bundle and should remain externally loaded.

## Verification Notes

- Final local browser smoke check passed with no broken images after sponsor logos were added.
- `vercel.json` includes a fallback rewrite so direct browser refreshes route back to the single-page app.
