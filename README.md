# Digital Legacy Registry

A small app for keeping a list of online accounts, noting what you would like done with them, and writing down trusted contacts.

## What it can do

- Add, edit, search and remove account records.
- Add trusted contacts and note what you intend to share with them.
- Save basic preferences for your plan.
- Export the records as JSON or print a summary.
- Restore the sample records.
- View a sample professional workflow.

## Before you use it

This is an early demo. It does not connect to social networks or other services. It cannot verify someone's death, get access to an account, change a username, or carry out any instructions.

The app saves records in your browser using `localStorage`. That data is not encrypted. JSON exports are not encrypted either. Use made-up information while trying it out. Don't enter passwords, recovery codes, identity documents, financial details, private messages, or real client information.

The professional page is only an example screen. It is not ready for use with clients.

## Run it on your computer

You need Node.js 20.19+ or 22.12+ and npm.

```bash
npm install
npm run dev
```

To check and build the app:

```bash
npm run typecheck
npm run build
npm run preview
```

## Publish with GitHub Pages

The repository has a workflow at `.github/workflows/deploy.yml`.

1. Open the repository's **Settings → Pages**.
2. Choose **GitHub Actions** as the source.
3. Push a change to `main`, or run the deployment workflow from the Actions tab.
4. GitHub will show the site address when the deployment finishes.

## Project files

- `src/App.tsx` — app screens and browser-side behavior.
- `src/styles.css` — styles.
- `src/main.tsx` — React entry point.
- `vite.config.ts` — Vite setup.
- `.github/workflows/` — build and deployment workflows.

## License

MIT. See [LICENSE](LICENSE).
