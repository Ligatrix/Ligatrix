# Ligatrix

Ligatrix builds custom business systems and hands them over. At the last payment, the repository, the code, the schema,
the runbook and the IP move to the client.

If you're a developer on a client team, this page covers what you'll receive, how changes reach your codebase, and
what the public repositories below are.

## What your team receives at the transfer

- **The repository**, moved into your organization with its full history.
- **The code.** Every line written for you, each change with its author and reviewer. The core platform it runs on stays
  Ligatrix's and is licensed to you permanently, with its full source included.
- **The schema.** Every table and field, and what each one holds.
- **The runbook.** How to start the system, fix it and restore it from a backup, kept current with every change. Before
  the transfer, a Ligatrix developer who has never seen the system ships a fix using the runbook alone.
- **Architecture notes.** What each part does and why, and every third-party dependency with its license.
- **The build record**, described below.
- **Every key and credential**, passed to your team.

## How changes are made

- Every change has a maker and a checker, named by role and recorded with the change.
- Tests run before a change ships, and their results are kept in the record.
- Dependency updates are reviewed like any other change and listed with their license.
- Access is granted by role. The record shows who granted it, who checked it and what it reaches. Our team holds no
  standing access to your data, and every access shows in the record.
- When a business rule or rate changes, the record keeps the old value beside the new one, with the date each took
  effect.

## After the transfer

Bugs in what we built are fixed for as long as the system runs. Your team decides who maintains it from there: you, or
us.

## Public repositories

These are small reference examples: a few hundred lines each, MIT-licensed, plain Node.js with no runtime
dependencies. They show the shape of our delivery records and patterns. They are not client code, and none of them contains
any.

| Repository | What it is | Try it |
|---|---|---|
| [ligatrix-starter-kit](https://github.com/Ligatrix/ligatrix-starter-kit) | A static operations workspace: intake, workflow states, an activity log and a handoff export | open `index.html` |
| [ligatrix-sdk](https://github.com/Ligatrix/ligatrix-sdk) | JavaScript helpers, with TypeScript types, for project contracts, intake events and evidence packs | `node examples/basic.mjs` |
| [ligatrix-ui](https://github.com/Ligatrix/ligatrix-ui) | Markup helpers for a status badge, a metric tile, an evidence list and a case card | `node examples/render.mjs` |
| [ligatrix-agent-runtime](https://github.com/Ligatrix/ligatrix-agent-runtime) | A deterministic step runner (request, action, checks, record, handoff) that makes no external calls by default | `node examples/run-workflow.mjs` |
| [ligatrix-mcp-servers](https://github.com/Ligatrix/ligatrix-mcp-servers) | An example JSON-RPC tool server that writes delivery-note and handoff skeletons; it reads no private files and makes no network calls | `node examples/test-evidence-server.mjs` |
| [ligatrix-cli](https://github.com/Ligatrix/ligatrix-cli) | Creates the contract, evidence and handoff files a project starts with | `node bin/ligatrix.mjs init-contract my-project` |
| [ligatrix-evals](https://github.com/Ligatrix/ligatrix-evals) | Runs labeled cases against expected outputs and required evidence | `node scripts/run-evals.mjs examples/intake-triage.eval.json` |
| [ligatrix-integrations](https://github.com/Ligatrix/ligatrix-integrations) | A JSON Schema for an intake event, a normalizer and a GitHub-issue intake pattern | `node scripts/normalize-intake.mjs examples/intake-event.json` |
| [ligatrix-security-toolkit](https://github.com/Ligatrix/ligatrix-security-toolkit) | A pre-publish scan for secrets, private keys, local paths and internal markers; exits 1 on a finding | `node scripts/scan-public-safety.mjs .` |
| [ligatrix-deploy-templates](https://github.com/Ligatrix/ligatrix-deploy-templates) | A Dockerfile, a Compose file and an nginx config for a static app, with a deploy checklist | `npm run check` |
| [ligatrix-cookbook](https://github.com/Ligatrix/ligatrix-cookbook) | Four workflow recipes: onboarding, approval, triage and a dashboard | `npm run check` |
| [ligatrix-llms-docs](https://github.com/Ligatrix/ligatrix-llms-docs) | `llms.txt` and the notes on what we publish and what we keep private | read `llms.txt` |

## What stays private

Client code and data, and the source of the core platform. Clients receive the core's full source under their license;
it isn't published here.

## Contact

Questions about a handover, or a security report: info@ligatrix.com
