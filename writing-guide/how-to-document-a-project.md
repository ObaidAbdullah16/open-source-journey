# How to Document a Project: My Playbook

If a line of code runs in production but no one can understand how to use it, it might as well not exist.

---

## 1. Know your reader

Ask:

- Who will land on this page?
- Are they a beginner or already familiar with the project?
- What problem are they trying to solve right now?

Tip: avoid words like “obvious” or “trivial.” If it were obvious, they wouldn’t be reading docs.

---

## 2. Make the README a map

A README should answer:

- What does this project do? (1–2 sentences)
- Who is it for?
- How do I run a quickstart example?
- Where do I get help?
- Where is CONTRIBUTING?

---

## 3. Structure beats style

Use headings, lists, and code blocks.
If someone can’t scan the doc and extract the “how,” rewrite it.

---

## 4. Use real examples

Include at least one copy/paste example:

- a working config or command
- short notes on what each key piece does

---

## 5. Test the instructions

If your doc says “run X,” run X from a clean setup.
Docs that don’t work waste time and hurt trust.

---

## 6. Don’t hide prerequisites

If you assume Git/Docker/Go, say it clearly at the top and link to installation docs.

---

## 7. Invite people in

A “How to get help” section matters.
People contribute more when the docs tell them where to ask questions and what information to include.

---

## 8. Keep a changelog (when it’s relevant)

A CHANGELOG helps users and contributors:

- it makes breaking changes visible
- it reduces confusion during upgrades

---

## Conclusion

When I’m unsure how to write something, I write it for my past self—the version of me who didn’t know the project yet.
