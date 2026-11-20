# Documentation

Index of the project documentation in `docs/`. Check here before writing a new document — the topic may already be covered.

## Architecture & design

| Document | Description |
|---|---|
| [adr/](./adr/README.md) | Architecture Decision Records — one file per significant design decision, with its own index |
| [indexer-architecture.md](./indexer-architecture.md) | How the indexer turns Soroban contract events into SQLite state: idempotency, cursor recovery, release accounting |
| [data-sourcing.md](./data-sourcing.md) | The indexer-first, RPC-fallback convention the frontend uses to read lock data |
| [notification-service.md](./notification-service.md) | Unlock-reminder notifier: cron worker, subscription API, schema, and email/webhook delivery |
| [storage-optimization.md](./storage-optimization.md) | Contract storage and rent optimizations for `token-locker` and `lp-locker` |
| [lp-pool-token-verification.md](./lp-pool-token-verification.md) | Best-effort pool-token verification in `lp-locker` and its security implications |

## Operations & security

| Document | Description |
|---|---|
| [incident-response.md](./incident-response.md) | Operator runbook for emergency `pause()` / `unpause()` on both contracts |
| [security-audit.md](./security-audit.md) | Contract threat model and security audit checklist |
| [troubleshooting.md](./troubleshooting.md) | Common user-facing errors (wallet, network, transactions, contract) with causes and fixes |

## Project & process

| Document | Description |
|---|---|
| [changes.md](./changes.md) | Hand-written rationale behind selected changes, by issue (the release list lives in [CHANGELOG.md](../CHANGELOG.md)) |
| [roadmap-notes.md](./roadmap-notes.md) | Internal planning notes on open feature gaps (batch lock creation, Arabic localization) |
| [bounty-payout-policy.md](./bounty-payout-policy.md) | Contribution and bounty payout policy |
| [bulk-actions-partial-failure.md](./bulk-actions-partial-failure.md) | Analysis of untested partial-failure handling in MyLocks bulk extend/transfer |
| [screenshots/](./screenshots/) | App screenshots embedded in the main README |
