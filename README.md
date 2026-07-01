# Dra. Wendy Cerecero — Portafolio

Sitio profesional para la **Dra. Wendy Yadira Cerecero Salas**, Cirujano Dentista (UVM, Cédula #5926257).

## Vista previa
Abre `index.html` en cualquier navegador moderno. No requiere build.

## Live
- **Production (Vercel):** https://dra-cerecero.vercel.app
- **Repo:** https://github.com/dra-wendycerecero/dra-cerecero-portfolio

## Branches

| Branch | Purpose |
|---|---|
| `main` | Development. All changes start here. |
| `prod` | Production. Merged PRs to `prod` trigger Vercel deployment. |

## Workflow

1. Develop on `main`
2. Push commits to `main`
3. Open PR: `main` -> `prod`
4. CI runs validation (file checks, no leaked tokens, meta tags)
5. Merge PR into `prod`
6. CD deploys to **Vercel** automatically

## Files
- `index.html` — the entire site (HTML + CSS + a small vanilla JS bundle)
- `favicon.svg` — monogram "WC"
- `61444.jpg` — profile photo
- `.github/workflows/prod.yml` — CI/CD pipeline

## CI/CD
- **Validate job**: runs on push to `main` — checks files exist, page size, meta tags, no leaked secrets
- **Deploy job**: runs when a PR is merged into `prod` — deploys to Vercel production

> **Note:** Requires repo secrets `VERCEL_TOKEN`, `VERCEL_ORG_ID`, and `VERCEL_PROJECT_ID`.
