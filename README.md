# Dra. Wendy Cerecero — Portafolio

Sitio profesional para la **Dra. Wendy Yadira Cerecero Salas**, Cirujano Dentista (UVM, Cédula #5926257).

## Vista previa
Abre `index.html` en cualquier navegador moderno. No requiere build.

## Live
- **Production:** https://dra-wendycerecero.github.io/dra-cerecero-portfolio/
- **Repo:** https://github.com/dra-wendycerecero/dra-cerecero-portfolio

## Branches

| Branch | Purpose |
|---|---|
| `main` | Development. All changes start here. |
| `prod` | Production. Pushed to main -> create PR main -> prod -> CI/CD deploys to Pages automatically. |

## Workflow

1. Develop on `main`
2. Push commits to `main`
3. Open PR: `main` -> `prod`
4. CI runs validation (file checks, no leaked tokens, meta tags)
5. On PR merge into `prod`, CD deploys to GitHub Pages automatically

## Files
- `index.html` — the entire site (HTML + CSS + a small vanilla JS bundle)
- `favicon.svg` — monogram "WC"
- `61444.jpg` — profile photo
- `.github/workflows/prod.yml` — CI/CD pipeline

## CI/CD
- **Validate job**: checks files exist, page size, meta tags, no leaked secrets
- **Deploy job**: runs only on push to `prod`, uploads artifact, deploys via official GitHub Pages action
