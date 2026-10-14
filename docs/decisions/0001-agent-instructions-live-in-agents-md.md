# 0001. Agent instructions live in AGENTS.md

- **Status:** Proposed
- **Date:** 2026-10-14

## Context

AI agents read different files: Codex, Copilot and Cursor read AGENTS.md;
Claude Code reads CLAUDE.md; Gemini CLI reads GEMINI.md. Copies drift apart.

## Decision

All instructions live in AGENTS.md. CLAUDE.md and GEMINI.md, where used,
contain only `@AGENTS.md`.

## Rejected

- A full copy per agent: they drift apart within weeks.

## Consequences

A rule is changed in one place. Rules that must never be broken are also
enforced by a hook and CI, not only written down.
