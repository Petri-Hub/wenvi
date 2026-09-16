# Security Policy

## Scope

Wenvi runs locally and handles secrets by design: it reads and writes `.env` files inside your project, and `export` writes them into a file encrypted with AES and a password you choose. It makes no network calls of its own, apart from `upgrade`, which runs `npm install -g wenvi`, and `docs`, which opens the repository in your browser. The realistic surface is how those files are handled and the dependency tree.

## Supported Versions

Only the latest version published on npm. Fixes ship as a new version.

## Reporting a Vulnerability

If you find a security issue, tell me privately instead of posting it publicly. **Don't open a GitHub issue.** Send an email to [fernando.petri01@gmail.com](mailto:fernando.petri01@gmail.com) with:

- What you found
- How to reproduce it
- Which version of wenvi, and which dependency if that's where it lives

## What happens next

1. I'll confirm the issue
2. I'll write and test a fix
3. I'll publish a new version to npm
4. I'll let you know when it's out
