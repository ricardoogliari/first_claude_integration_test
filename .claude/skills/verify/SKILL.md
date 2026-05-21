---
name: verify
description: Run lint and tests, then summarize pass/fail. Use after making changes to confirm nothing is broken.
---

Run the following commands in sequence and report results:

1. `npm run lint` — ESLint via Next.js config
2. `npm run test` — Vitest unit + component tests

For each command, report:
- Pass or fail
- Any errors or warnings (show the relevant lines, not the full output)

End with a one-line summary: "All checks passed" or a count of what failed and which commands to fix.
