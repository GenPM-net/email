# @core/email

[![genpm](https://api.genpm.net/v1/badge/@core/email.svg)](https://genpm.net/p/@core/email) ![license](https://img.shields.io/badge/license-MIT-blue)

> Transactional email with typed React Email templates: Resend, SMTP or console in dev

A [GenPM](https://genpm.net) module: **source code + AI rules + MCP config**, injected into your project instead of hidden in `node_modules`. The code lands in `src/lib/email`, pinned to a verified commit, and you own it.

## Install

```bash
genpm add @core/email
```

No genpm yet? `curl -fsSL https://genpm.net/install.sh | sh` (macOS/Linux), `irm https://genpm.net/install.ps1 | iex` (Windows), or one-off with `npx @genpm-net/cli add @core/email`.

Or let your AI agent do it: run `genpm mcp setup` once, then ask *"add @core/email with genpm"* in Claude Code, Cursor, VS Code, Windsurf, Codex or Gemini CLI. It shows you a dry-run plan before writing anything.

## What it does

Transactional email with typed templates: `sendEmail('welcome', { to, props })`. Providers: Resend (default), SMTP
(optional, via `nodemailer`) and a console provider for development. Templates use React Email. No marketing lists,
no queues, no tracking pixels.

## At a glance

- **npm dependencies** (proposed, never installed without asking): `resend`, `@react-email/components`, `@react-email/render`, `react`, `@types/react`
- **Environment variables** (added to `.env.example`): `RESEND_API_KEY`, `EMAIL_FROM`, `APP_NAME`
- **AI rules**: [`AGENTS.md`](AGENTS.md), loaded by your agent only when it works in `src/lib/email`

## Security

GenPM installs a 40-character commit SHA (never a branch), verifies an Ed25519-signed manifest, never runs install scripts and scans AI rules for prompt injection. Details: [genpm.net/docs/security](https://genpm.net/docs/security).

## License

MIT — see [LICENSE](LICENSE). Browse the full catalog at [genpm.net](https://genpm.net).
