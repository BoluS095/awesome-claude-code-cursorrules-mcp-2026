# AGENTS.md — Multi-Agent Swarm & Tool-Batching Rules (2026)

1. **Batch independent calls.** Issue independent reads, searches, and edits in parallel each turn.
2. **Single-owner module boundaries.** Keep provider protocols and payload parsing inside the owning module; share narrow normalized contracts.
3. **Idempotent state transitions.** Every background job, webhook, and fulfillment worker must be safely re-entrant.
4. **Explicit failure handling.** Never swallow errors with empty catch blocks on critical write paths.
5. **Evidence expires after edits.** Re-run affected verification checks after any code change or rebase.
