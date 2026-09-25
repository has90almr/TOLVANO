# TOLVANO WCC Static App

Private owner UI artifact for `app.tolvano.com`.

- Static HTML/CSS/JS only.
- No service-role key, OpenAI key, provider secret, or worker credential is present.
- Browser uses the Supabase publishable key only.
- WCC data is returned only by the JWT-protected `tolvano-wcc-control` Edge Function after a private OWNER binding check.
- Access token is kept in sessionStorage only; no refresh token is persisted.
- Control/mutation/external-effect actions remain disabled until Full Executable closure and independent review.
- Configure the hosting project root directory to this `wcc-app` folder.
