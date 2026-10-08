# PASION on GitHub Pages

This project contains a React/Vite frontend and an optional Python backend. GitHub Pages can host the **frontend only**; it cannot execute the Python backend.

## Deploy the real UI

1. Push this repository to GitHub.
2. Open **Settings → Pages**.
3. Under **Build and deployment → Source**, select **GitHub Actions**.
4. Push to the `main` branch (or run the workflow manually).
5. The included `.github/workflows/deploy.yml` installs the Node dependencies and runs `npm run build:github`.

Do **not** select **Deploy from a branch** for the source repository. That mode would serve `index.html` and `src/main.jsx` directly, and browsers cannot execute the JSX/SCSS source files. That is the usual cause of a blank/white page.

## Static demo limitations

The visual design and frontend interactions remain intact. On GitHub Pages, account/session behavior is browser-local demo behavior. Secure password changes, email recovery, administrator persistence, document upload/OCR, and other Python-backed operations require the full backend deployment.

## Demo login

- Email: `demo@solvai.com`
- Password: `SolvAI2024!`
