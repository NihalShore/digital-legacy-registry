# Digital Legacy Registry

**Your digital life. Your rules. Your legacy.**

Digital Legacy Registry is an open-source prototype for documenting online accounts, recording personal legacy preferences, and identifying trusted contacts. It treats a username and a human identity as different things: a platform may eventually release a handle under its own policies, but a person's identity, history, and account ID must never be transferred to a new owner.

> **Prototype warning:** This is a front-end demonstration, not a secure digital vault or a service for estate, incapacity, or post-death administration. Use fictional data only. Do not enter passwords, recovery codes, identity documents, financial information, private messages, or real sensitive personal information.

## What works in v0.1.0

- Add, edit, search, and remove digital account records.
- Record a platform, username or identifier, optional profile URL, lifecycle status, instruction, and notes.
- Record trusted contacts and intended sharing scope. No invitations are sent and no access is granted.
- Set planning preferences, including a clear non-transfer principle for human identity.
- Export a portable JSON report or print a summary.
- Reset the browser to fictional sample data.
- Explore a read-only professional-workflow concept using fictional client cases.
- Responsive layout for desktop, tablet, and mobile.

## Important boundaries

This prototype does **not**:
- Connect to Instagram, Facebook, X, TikTok, Google, Apple, GitHub, or another platform.
- Change, claim, recycle, reserve, or transfer usernames.
- Authenticate a person, verify a death, assess legal authority, or determine inheritance rights.
- Send a trusted-contact invitation or give a contact access to an external account.
- Store passwords or secrets.
- Encrypt browser records, synchronize across devices, or provide a backend account.
- Automatically delete, memorialize, preserve, or transfer anything on another service.

Records are saved to the current browser's `localStorage` in readable form. Clearing browser data removes those records. JSON exports are also unencrypted. The professional page is a design preview only and must not be used with client data.

## Run locally

Requirements: Node.js 20.19+ or 22.12+ and npm.

```bash
npm install
npm run dev
```

Open the local URL printed by Vite.

Create a production build:

```bash
npm run typecheck
npm run build
npm run preview
```

## Deploy free with GitHub Pages

This repository includes `.github/workflows/deploy.yml`.

1. Push the project to GitHub using the `main` branch.
2. In **Settings → Pages**, set the source to **GitHub Actions**.
3. Push to `main` or run the **Deploy to GitHub Pages** workflow manually.
4. After the workflow succeeds, GitHub will show the published site URL in Pages settings and the workflow deployment.

The Vite build uses relative asset paths so it can run from a repository subpath.

## Data model

The browser record contains:
- `accounts[]`: platform, username, URL, preferred action, lifecycle state, and optional notes.
- `contacts[]`: name, email, relationship, and an intended sharing scope.
- `preferences`: planning-level directives selected by the user.

No remote API or database is configured in this release.

## Product principles

1. **Portable records:** users should be able to export their information without being locked into one provider.
2. **Identity is not a username:** an available handle is not permission to inherit another person's identity or history.
3. **User-directed sharing:** a professional or contact should see only what the individual explicitly authorizes.
4. **No credential collection:** the registry should not ask users for third-party passwords.
5. **Platform authority is respected:** account actions and username availability remain subject to each provider's official process and policies.
6. **Privacy is not a luxury:** basic export and deletion controls should not be paywalled.

## Security

Read [SECURITY.md](SECURITY.md) before using or contributing to the prototype.

## License

MIT. See [LICENSE](LICENSE).
