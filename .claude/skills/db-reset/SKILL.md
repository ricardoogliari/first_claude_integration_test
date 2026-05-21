---
name: db-reset
description: Reset the SQLite database to its initial state. Only invoke when the user explicitly asks to reset the database.
disable-model-invocation: true
---

This skill resets the project database. It is destructive — all data will be lost.

Steps:
1. Warn the user: "This will delete all data in `prisma/dev.db` and re-run migrations. Are you sure?"
2. Wait for confirmation before proceeding.
3. Run: `npm run db:reset`
4. Report success or any errors.
