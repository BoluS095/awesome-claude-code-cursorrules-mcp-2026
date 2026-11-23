# CLAUDE.md — Senior Full-Stack Engineering Operating Contract (2026)

## Core Discipline
1. **Read before editing.** Always inspect full types, schemas, and adjacent tests before proposing changes.
2. **Red -> Green TDD.** Reproduce bugs with a failing test first, apply the smallest clean fix, and confirm green.
3. **Zero fabricated telemetry.** Never claim tests, builds, or HTTP checks passed without observed exit code 0.
4. **Sync contracts end-to-end.** Schema -> shared types/validators -> API route/service -> UI client -> tests.
5. **Security by default.** Validate every external input with Zod/Pydantic, use parameterized SQL, enforce auth/tenant scope on every mutation, and never commit secrets or disable TLS/auth.

## Output Format
- Lead with the root cause or concrete diff summary.
- Keep diffs surgical; avoid unrelated refactors.
- List exact verification commands run and any remaining gaps.
