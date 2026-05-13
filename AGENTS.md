# AGENTS.md

Guidance for Codex, Copilot coding agent and other AI coding agents working on this repository.

## Core coding-agent rules

These rules are adapted from the Karpathy-style coding-agent guidelines and the project CODEX.md rules.

### 1. Think before coding

- Inspect the real repository before changing files.
- Do not assume missing requirements silently.
- State assumptions when they affect implementation.
- If a request has several meanings, choose the safest small interpretation and say so, or ask when the wrong choice would be costly.
- Push back when a simpler or safer approach exists.

### 2. Simplicity first

- Write the minimum code that solves the task.
- Do not add speculative features, abstractions, configuration, or frameworks.
- Prefer clear, boring code over clever code.
- If the change becomes large, re-check whether a smaller change is enough.

### 3. Surgical changes

- Touch only files directly needed for the task.
- Do not refactor, rename, reformat, or clean adjacent code unless required.
- Match existing style.
- Preserve unrelated user changes.
- Remove only unused code created by your own change.

### 4. Goal-driven execution

- Convert the task into verifiable success criteria.
- For bugs, reproduce the bug first when practical, then fix it.
- Run the smallest relevant check before claiming completion.
- Report changed files, verification performed, and anything not tested.

## Project profile

This repository contains an interactive compatibility map/table for power-tool batteries based on practical forum data.

Main files:
- `index.html` — GitHub Pages interface;
- `data/relations.csv` — compatibility relations;
- `forum-post.md` — prepared forum post text.

## Project-specific constraints

- Treat the data as user-reported practical evidence, not official manufacturer compatibility.
- Do not invent compatibility, adapter behavior, electrical safety, or battery protection details.
- Keep warnings about connector shape, polarity, contacts, thermistor/ID pins, current capability, overdischarge and overheating protection.
- Prefer editing `data/relations.csv` surgically instead of rewriting all data.
- Do not remove uncertainty markers or evidence notes unless the source justifies it.
- Keep the project usable as a static GitHub Pages site unless explicitly requested otherwise.

## Useful checks

This project may be mostly static. Before final response:
- inspect the changed page/table in a browser when possible;
- if no automated test exists, say so directly;
- state changed files and what was manually checked.
