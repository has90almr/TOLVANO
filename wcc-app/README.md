# TOLVANO WCC Static App

Private owner UI artifact for `app.tolvano.com`.

- Static HTML/CSS/JS only.
- No service-role key, OpenAI key, provider secret, worker credential, or database password is present.
- Browser uses the Supabase publishable key only.
- WCC data is returned only by the JWT-protected `tolvano-wcc-control` Edge Function after a private OWNER binding check.
- Access token is kept in sessionStorage only; no refresh token is persisted.
- Control/mutation/external-effect actions remain disabled until Full Executable closure and independent review.
- Render Blueprint lives at repository root as `render.yaml`.
- Render service root is `wcc-app`; the static publish path is the directory itself.
- Intended production origin: `https://app.tolvano.com`.
- DNS is currently hosted by Spaceship. The app subdomain is intentionally not created until the static host target exists.
