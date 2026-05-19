# Notes — Meshery relationships (draft)

These notes are here so I can pick relationship work that doesn’t overlap existing PRs.

## What I’m trying to avoid

- Working on a “master issue” without a clear sub-scope
- Duplicating relationship pairs that are already in an open PR
- Submitting a PR without proof (Kanvas screenshot/video)

---

## Quick mental checklist for relationships

Before writing a relationship definition, I want to answer:

- What’s the real-world interaction?
- Is it **hierarchical** (parent/child) or an **edge** (reference/integration)?
- What direction makes sense in the graph?
- Is there an existing pattern in the repo I should copy?

---

## Candidate scopes (examples)

I’ll pick one scope based on what’s NOT already covered by active PRs.

### Option A: Azure Batch — Pools/Jobs/Tasks (expand beyond BatchAccount)

Possible relationships:

- BatchAccount → BatchPool (hierarchical parent)
- BatchPool → BatchJob (reference or hierarchical depending on model)
- BatchJob → BatchTask (hierarchical parent)
- BatchPool → VirtualNetwork/Subnet (network)
- BatchPool → ManagedIdentity (identity)

Plan:

- If maintainers prefer it: create a sub-issue first and reference #18496
- Keep PR small: 2–6 relationships

### Option B: A single AWS service family (not crowded)

Examples:

- CloudFront → S3 (origin)
- CloudFront → WAF (security)
- CloudFront → ACM certificate (TLS)
  Or pick a less-touched AWS service and add 2–4 core relationships.

### Option C: One GCP service area (if less activity)

- Cloud Run ↔ Cloud SQL
- Cloud Run ↔ Secret Manager
- Cloud Run ↔ Pub/Sub

---

## Proof for reviewers (how I’ll do it)

### Screenshot plan

- Open Meshery → Kanvas
- Create a small design with 2–3 components
- Draw/confirm relationships
- Screenshot showing the relationship lines and component names

### Short video plan (30–60 seconds)

- Start recording
- Open Kanvas design
- Add the components
- Connect them (or show connections already visible)
- Stop recording
- Upload to PR comment (or link from a file)

---

## PR hygiene notes

- Keep relationship file names consistent with repo conventions
- Keep metadata descriptive (displayName, description)
- Mention exactly what relationships are added in PR description
- Link to the issue/sub-issue clearly
