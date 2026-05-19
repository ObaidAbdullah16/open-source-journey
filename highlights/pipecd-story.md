# PipeCD: Plugin Development Book & Docs DX — My Understanding & Plan

## Project problem (in my words)

PipeCD v1 has a plugin-based architecture, but the best learning resource for plugin development is currently only available in Japanese. That blocks a lot of potential contributors and slows adoption.

This project is about publishing an English Plugin Development Book inside PipeCD docs, adding practical pipedv1 examples, improving documentation experience, and producing supporting content (blogs/videos/talks).

The core problem isn’t just “translation.” It’s onboarding for a global audience.

## What “success” looks like

A motivated engineer should be able to:

- open the docs,
- follow the English book,
- build a simple plugin,
- understand how pipedv1 uses plugins,
- and find examples that match current usage.

If someone can realistically go from “interested” to “first plugin PR” faster, the project is working.

## My understanding of PipeCD (high level)

My current mental model:

- PipeCD is a continuous delivery system.
- piped runs agent-side and executes deployment logic.
- plugins make it possible to support different platforms and workflows.
- docs and examples are the bridge between architecture and actual usage.

Docs DX matters because even good content fails if:

- it’s hard to find,
- navigation is unclear,
- steps don’t work,
- or examples are outdated.

## My approach to solving the project problem

### 1) Make the English book structured and easy to maintain

I’d avoid one long page. I’d keep it chapter-based:

- overview / table of contents
- architecture and mental model
- first plugin walkthrough
- configuration + lifecycle
- testing + debugging

Each chapter should include:

- short explanations
- real snippets
- “common mistakes” callouts
- checkpoints so readers know they’re on track

### 2) Keep it accurate to the current repo

If I write docs that don’t match the repo, it’s worse than no docs. So I’d:

- verify commands and paths
- check APIs against the current codebase
- keep examples minimal but runnable
- link to existing plugins in the repo

### 3) Add practical pipedv1 examples

Examples should look like something people actually deploy:

- repo layout
- plugin config
- what a platform team would run, not just toy cases

### 4) Improve discoverability

Small doc improvements can unlock the whole project:

- consistent “where to go next” links
- clear “how to run docs locally” instructions
- predictable structure so new chapters fit naturally

## What I can contribute early

Even before deep plugin implementation, I can contribute by:

- drafting the book structure and the first chapters
- doing small docs DX improvements that reduce confusion
- validating every instruction by running it and fixing the parts that don’t work

## Why I’m interested in this project

I like building learning material that makes complex systems approachable. PipeCD’s plugin architecture is valuable, but without English resources and practical examples it’s harder for the community to grow. I want to help reduce that friction.
