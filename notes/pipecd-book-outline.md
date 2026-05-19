# Notes — PipeCD Plugin Development Book (English) outline (draft)

These are rough notes for structuring the English Plugin Development Book. Not final text.

## Goal

Make it possible for an English-speaking engineer to:

1. understand the plugin architecture,
2. build a small plugin,
3. test/debug it,
4. and know what a “good PR” looks like.

---

## Proposed structure

### 0. Overview

- What this book covers
- Who it’s for
- Prerequisites (Go, Git, basic PipeCD concepts)
- How to run docs locally (if relevant)
- How to follow along with code/examples

### 1. Architecture & mental model

- What plugins are in PipeCD v1
- Where plugins run (piped side)
- How Control Plane ↔ piped ↔ plugin communicate
- What problems plugins solve (platform diversity)
- Link to in-repo examples

### 2. Build your first plugin (minimal)

- Create a simple plugin that implements a small interface
- Basic config
- Run locally (or in a dev environment)
- Confirm it’s called by piped

### 3. Plugin configuration & lifecycle

- How configuration is loaded
- Versioning considerations
- Error handling patterns
- Logging recommendations

### 4. Testing & debugging

- Unit tests
- Integration tests (if available)
- How to debug plugin failures
- Common mistakes section

### 5. Real-world example patterns (optional, later)

- “production-ish” layouts
- how teams structure plugin repos
- how to document plugin configuration for users

---

## Notes to avoid doc rot

- Verify file paths and commands against the repo before writing
- Keep “copy/paste” blocks minimal and correct
- Prefer linking to stable sources (official docs) instead of re-explaining everything
