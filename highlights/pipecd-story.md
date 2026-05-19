# PipeCD: Plugin Development Book & Docs DX — My Understanding & Plan

## Project problem (in my own words)

PipeCD has a powerful plugin-based architecture (especially in v1), but the best learning resource for building plugins is currently only available in Japanese. That creates a real barrier: many contributors and adopters can’t learn plugin development properly.

This project aims to:

- translate and expand the Plugin Development Book into English,
- publish it inside PipeCD docs,
- add real pipedv1 examples,
- and improve docs experience so contributors can actually find and use the content.

It’s not just translation. It’s onboarding.

## What I believe “success” looks like

A motivated engineer should be able to:

- open PipeCD docs,
- follow an English Plugin Development Book,
- build a simple plugin,
- understand how pipedv1 uses plugins,
- and find real examples that match modern usage.

If a new contributor can go from “curious” → “first plugin PR” faster, the project is successful.

## My understanding of PipeCD and where this work fits

From what I understand:

- PipeCD is a continuous delivery system.
- A key architectural idea is that deployments can target many platforms by using plugins.
- piped is an agent-side component that runs deployment logic.
- The docs and examples act as the bridge between the architecture and actual adoption.

The project also includes “Docs DX” which matters because:

- even great content fails if navigation is confusing,
- readers can’t find what they need,
- and examples are missing or outdated.

## My approach to solving the project problem

### 1. Build the English book as a structured docs section

Instead of one long page, I would keep it as a chapter-based structure:

- Overview / Table of contents
- Chapter 1: plugin architecture and mental model
- Chapter 2: first plugin walkthrough
- Chapter 3: config and lifecycle
- Chapter 4: testing and debugging

Each chapter should include:

- short explanations
- real code snippets
- “common mistakes” callouts
- small checkpoints so the reader knows they’re on track

### 2. Expand beyond translation

Translation is useful, but the content should also fit the current PipeCD reality:

- confirm APIs, commands, and folder paths match current repo
- update examples so they compile and run
- add links to existing plugins in the codebase
- document what changed since earlier versions

### 3. Add examples that match real adoption patterns

pipedv1 examples should not be “toy” examples only. They should show:

- typical repo layout
- plugin configuration
- how a platform team would actually run it

### 4. Improve discoverability and contributor experience

Small docs improvements can have big payoff:

- better navigation and linking between sections
- consistent terminology and “where to go next”
- clear “how to run docs locally” steps for contributors
- standard doc structure so future additions stay consistent

## What I can contribute early (before deep plugin work)

Even before writing advanced plugin code, I can contribute by:

- producing a clean English structure for the book
- writing the first chapters in a way that is easy to review
- adding “docs DX” improvements (navigation, clarity, consistent templates)
- validating the instructions by running them and fixing what doesn’t work

## Why I’m choosing this project

I like building learning material that makes complex systems approachable. PipeCD’s plugin architecture is valuable, but without English resources and examples, it stays locked behind a language barrier.

My goal is to help new contributors ship their first plugin faster—and make the docs feel like a real product, not an afterthought.
