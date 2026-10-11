# Agent instructions

This repository currently contains the local, read-only CRM agent package. The
Twenty operations extraction is a separate, pending work unit.

Load `.agents/skills/cominorsa-crm-agent/SKILL.md` before working on the CLI,
MCP server, Twenty read adapter, or agent-facing CRM behavior.

Never infer live CRM authorization from available credentials. Do not inspect
ambient secrets, contact a CRM, import customer data, or add write/outreach
capabilities without explicit authorization for the destination, operation,
and credential/session. Offline checks use fixtures only.

Use Node.js 22.18+ and pnpm 11.25.0. `pnpm --ignore-workspace check` runs the package tests,
strict typecheck, and credential-free tool discovery. Keep source, tests, and
documentation together when changing behavior.
