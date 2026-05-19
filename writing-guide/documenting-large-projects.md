# Documenting Large Projects: What I Keep in Mind

When a project is big (multiple teams, many modules, lots of history), documentation needs to work like a navigation system. You’re not writing for one person reading start-to-finish. You’re writing for people who arrive stressed, busy, and mid-problem.

Here’s how I approach documentation for large projects.

---

## 1. Don’t try to “document everything”

Large projects die by documentation sprawl. If you try to write everything:

- it won’t stay updated,
- it will contradict itself,
- and users stop trusting it.

Instead, document the most common user journeys.

---

## 2. Identify your “entry points”

Most readers want one of these:

- installation / setup
- first working example
- reference docs
- troubleshooting
- contributing

If those entry points are weak, everything else feels harder.

---

## 3. Write like the repo is a city

Think of docs like city signs:

- clear routes
- consistent labeling
- short paths to key destinations

For example:

- a “Getting Started” path
- an “Advanced Topics” section
- a “Reference” section
- and “Troubleshooting”

---

## 4. Make docs modular

Long pages are hard to maintain. I prefer:

- small focused pages
- clear titles
- predictable structure
- heavy linking between pages

Modular docs also make PR reviews easier.

---

## 5. Don’t break the reader’s mental model

If you introduce a term, keep using it consistently.
If the project uses “Policy” and “Rule,” don’t randomly switch to “Check” or “Validation unit.”

Consistency is underrated.

---

## 6. Include examples that match real-world usage

In big projects, “Hello World” examples help, but they are not enough.

The best docs include:

- minimal example (to get started)
- realistic example (how teams actually use it)
- common failure example (what breaks and how to fix it)

---

## 7. Make troubleshooting a first-class feature

Good troubleshooting saves maintainers time.

I like to include:

- common error messages
- why they happen
- how to fix them
- how to gather logs / debug info

---

## 8. Protect docs from “rot”

Docs rot when:

- file paths change
- commands change
- default config changes
- examples stop compiling

A simple rule: if docs contain commands, someone should be able to run them from scratch.

Even if automated tests aren’t possible, you can still manually validate the steps before merging.

---

## 9. Review docs like a user, not like an author

Before calling docs “done,” I try to:

- open it on a fresh machine mindset
- copy commands into a terminal
- click every link
- scan it in under a minute and see if the structure makes sense

If it’s hard to scan, it’s hard to use.

---

## Final note

In big projects, docs are part of the product. Good docs lower the support burden, make onboarding faster, and help the project scale beyond a small group of maintainers.
