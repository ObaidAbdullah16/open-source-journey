# Documenting Large Projects: What I Keep in Mind

In a big project (lots of modules, history, and contributors), documentation needs to work like navigation. People don’t read everything—they arrive with a goal, a bug, or a deadline.

Here’s what I keep in mind when writing docs for projects at this scale.

---

## 1. Don’t try to document everything

If you try to cover everything, the docs won’t stay updated and people stop trusting them.

Instead: document the most common user journeys first.

---

## 2. Make the entry points obvious

Most readers are looking for one of these:

- installation / setup
- first working example
- reference docs
- troubleshooting
- contributing

If those are weak, the rest of the docs won’t matter.

---

## 3. Treat the repo like a city

Docs should help readers move quickly:

- clear routes
- consistent labels
- short paths to key destinations

A few well-maintained hubs beat a hundred scattered pages.

---

## 4. Keep pages small and link them well

Long pages are harder to keep correct.

I prefer:

- small focused pages
- predictable headings
- strong linking between related topics

This also makes PR review easier.

---

## 5. Protect the reader’s mental model

If the project uses “Policy” and “Rule,” don’t casually switch to different terms. Consistency makes docs easier to understand and easier to search.

---

## 6. Use examples that match real usage

The best docs usually have:

- a minimal example (to start)
- a realistic example (how teams actually run it)
- a failure example (what breaks and how to fix it)

---

## 7. Treat troubleshooting as part of the product

Troubleshooting sections reduce maintainer load.

Good troubleshooting includes:

- common error messages
- why they happen
- how to fix them
- what logs/info to gather before asking for help

---

## 8. Fight documentation rot

Docs rot when commands change, defaults change, and examples stop working.

If docs include commands, someone should be able to run them from scratch. If that’s not testable automatically, it still needs manual verification before merging.

---

## 9. Review docs like a user

Before calling docs “done,” I try to:

- scan it in under a minute (does the structure work?)
- click every link
- copy/paste commands (do they work?)
- check if the reader can find the “next step”

---

## Final note

In large projects, documentation is part of how the project scales. Good docs save time for users and maintainers.
