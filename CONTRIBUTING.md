# Contributing

Thanks for helping improve Digital Legacy Registry. Contributions should make the product safer, clearer, more accessible, and more useful without weakening user control.

## Development

1. Fork the repository and create a focused branch.
2. Install dependencies with \`npm install\`.
3. Run \`npm run dev\` while developing.
4. Run \`npm run typecheck\` and \`npm run build\` before opening a pull request.
5. Describe the user problem, the change, and how it was tested.

## Product guardrails

- Do not add password, recovery-code, or secret collection.
- Do not imply that the app can control third-party accounts or release usernames.
- Do not treat inactivity as proof of death or incapacity.
- Keep all sample identities fictional.
- Keep basic export and deletion controls available without payment.
- Do not add analytics, trackers, or remote persistence without an explicit privacy review and documentation.
- Professional access must be explicit, scoped, and revocable before it is implemented.

## Pull requests

Keep pull requests small and focused. Include screenshots for visual changes and note any privacy or security implications. Update documentation when behavior or setup instructions change.
