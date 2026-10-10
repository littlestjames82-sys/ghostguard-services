# GhostGuard Services

The service side of [GhostGuard](https://github.com/littlestjames82-sys/ghostguard)
— Ghost Developer Studio's governance layer for agents that act in the real
world. **All pricing in this repo is DRAFT. GhostGuard produces records and
gates effects; it certifies nothing, and neither do these services.**

By **Ghost Developer Studio**. MIT licensed.

## What's here

### `audit/` — Agent Governance Audit (service pack)

A fixed-scope audit engagement, packaged end-to-end:

- `SERVICE_SHEET.md` — what the audit is, the 5 fixed-scope steps
  (intake → action inventory/classification → GhostGuard policy simulation
  → report → walkthrough), deliverables, and what the client must provide.
- `INTAKE.md` — the exact intake instrument (with a hard rule: clients
  never send real secrets — type + length only).
- `REPORT_TEMPLATE.md` — the fill-in audit report skeleton, driven by a
  real simulation trail.
- A **worked example**: a fictional client (`example-report.md`, labelled
  FICTIONAL throughout) whose 17-action inventory was evaluated through
  the real GhostGuard engine by `generate-example-trail.mjs`, producing
  `example-trail.jsonl` and `example-summary.json` — every number in the
  example report is copied from that real output.

### `whitelabel/` — White-Label Audit Portal (prototype)

- `portal.html` — a single-file, no-server prototype of the trail /
  approvals view an agency can show its own clients under its own
  branding (agency name, logo text, accent color swappable via a small
  config or URL parameters), with a "Powered by GhostGuard" line kept.
  Demo state is the same fictional 17-record trail.
- `SPEC.md` — how this becomes the hosted Agency-tier feature:
  per-agency subdomains, client workspaces, real decision appends,
  approver identity, server-side redaction.

See `REPORT.md` for the build report and the list of decisions that remain
the studio's (pricing, any public listing, sending the sheet to a client).
