# Ligatrix

**We build the systems your company runs on, and hand you the keys.**

Ligatrix designs and builds custom internal systems for companies: operations portals, workflow and approval tools, dashboards,
integrations between the software you already use, and client portals. When the work is done, the code, the documentation and every
access move to you.

[Book a 30-minute call](https://ligatrix.com/contact/sales) · [ligatrix.com](https://ligatrix.com) · info@ligatrix.com

## What we build

- **Operations portals**: requests, approvals and records in one place, with a clear owner for every step.
- **Workflow tools**: the process your team runs on spreadsheets and email, turned into software with an audit trail.
- **Dashboards**: the numbers leadership asks for every week, live and from the source.
- **Integrations**: your CRM, helpdesk, accounting and code platforms speaking to each other through one consistent shape.
- **Client portals**: a place where your customers see status, documents and next steps without emailing you.

## What you own at handover

Every system we build ends with a complete handover, so you are never locked in:

| You receive | Where to see an example |
|---|---|
| The repository, in your own GitHub, with its full history | [ligatrix-demo-portal](https://github.com/Ligatrix/ligatrix-demo-portal) |
| Architecture notes and decision records | [handover example: architecture](https://github.com/Ligatrix/ligatrix-handover-kit/tree/main/examples/corvane-portal) |
| A runbook: start, deploy, back up, restore, rotate keys | [handover example: runbook](https://github.com/Ligatrix/ligatrix-handover-kit/tree/main/examples/corvane-portal) |
| Deployment files for your own infrastructure | [ligatrix-deploy](https://github.com/Ligatrix/ligatrix-deploy) |
| The test suite, running in CI on every change | every repository below |
| An access-transfer checklist: accounts, DNS, secrets, admins | [ligatrix-handover-kit](https://github.com/Ligatrix/ligatrix-handover-kit) |

## Start here

| Repository | What it is |
|---|---|
| [ligatrix-demo-portal](https://github.com/Ligatrix/ligatrix-demo-portal) | A working operations portal for a fictional distributor: intake, approvals, workflow states, activity log, dashboard, handover export. Runs with `npm start`. |
| [ligatrix-handover-kit](https://github.com/Ligatrix/ligatrix-handover-kit) | The handover package a client receives, with a CLI that creates and checks it, and a complete worked example. |
| [ligatrix-components](https://github.com/Ligatrix/ligatrix-components) | A framework-free, accessible component kit for internal tools and dashboards, with design tokens and a one-page gallery. |
| [ligatrix-connectors](https://github.com/Ligatrix/ligatrix-connectors) | Adapters that bring webhooks, CRM, helpdesk, GitHub and CSV events into one validated shape, with signature checks and deduplication. |
| [ligatrix-deploy](https://github.com/Ligatrix/ligatrix-deploy) | How we ship: a hardened container, PostgreSQL, nginx with security headers, backups and restores, all checked in CI. |
| [ligatrix-secret-scan](https://github.com/Ligatrix/ligatrix-secret-scan) | A command-line scanner that keeps credentials out of repositories, with SARIF output for code scanning. |

## How we work

- Every change is reviewed and tested before it ships, and every repository runs its tests in CI.
- Documentation is part of the delivery, not an afterthought: architecture notes, a runbook and decision records ship with the code.
- We build on open, well-understood technology, so any competent team can run what we hand over.
- Security is designed in from the first commit: least-privilege access, secrets kept out of code, dependencies reviewed.

Every repository here is MIT-licensed. Issues and pull requests are welcome.

---

**Have a system you need built?** [Book a 30-minute call](https://ligatrix.com/contact/sales). Security reports: info@ligatrix.com.
