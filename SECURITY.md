# Security policy

## Current security status

Digital Legacy Registry v0.1.0 is a static prototype. It is **not suitable for real personal or client records**. Data is stored as readable JSON in browser `localStorage`; it is not encrypted, authenticated, backed up, or synchronized. JSON exports are also unencrypted. The professional workflow screen is fictional and read-only.

Do not submit real sensitive information to this prototype. Do not use it to make legal, estate, incapacity, or post-death decisions.

## Reporting a vulnerability

Please do not publish details of a suspected vulnerability in a public issue. Use GitHub's private vulnerability reporting feature if enabled for the repository, or contact the maintainer privately through the contact details listed on the repository profile.

Include the affected version, impact, and steps to reproduce. Do not include real personal data in a report.

## Before production use

A production service would require, at minimum, a documented threat model, independent security review, encryption design, authenticated access, tenant isolation, scoped and revocable permissions, audit logs, secure backups, retention and deletion procedures, incident response, and jurisdiction-specific legal review. None of these should be inferred from the current prototype.
