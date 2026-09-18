# BizLedger — GitHub Pages deployment

This project is configured for deployment with GitHub Actions and GitHub Pages.

## 1. Create the repository
Create a GitHub repository named `bizledger` (or another name you prefer), then upload/push the contents of this project to the repository's `main` branch.

## 2. Enable GitHub Pages
In the repository, open **Settings → Pages**. Under **Build and deployment → Source**, select **GitHub Actions**.

## 3. Push to `main`
The included `.github/workflows/deploy.yml` will install dependencies, run `npm run build`, and deploy `dist` automatically.

For a repository named `bizledger`, the site URL will be:
`https://YOUR-GITHUB-USERNAME.github.io/bizledger/`

The Vite configuration automatically sets the `/bizledger/` base path during GitHub Actions builds.

## Local development
```bash
npm install
npm run dev
```

## Production build
```bash
npm run build
npm run preview
```
