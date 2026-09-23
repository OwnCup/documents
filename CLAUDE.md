# CLAUDE.md — OwnCup `documents`

Guidance for Claude Code / autopilot agents working in this repository.

## ⚠️ This repository is PUBLIC — public documents ONLY

`OwnCup/documents` is a **public** repository. It is published (GitHub Pages / the
landing site) and is visible to anyone on the internet — including every branch and the
full git history, not just `main`.

**Only public-facing content may live here**, for example:

- Privacy policy (`privacy_policy.md`, `privacy_policy_bg.md`)
- Cookie policy (`cookie_policy.md`)
- Terms / contract offers (`OWNCUP_Contract_Offer_*.docx`)
- Account removal page (`remove-account.html`) and public landing assets (`favicon.*`)

### Never commit internal documents or reports here

Do **not** commit — on any branch, including feature branches — any internal material,
such as:

- implementation / migration / account-deletion plans
- readiness, verification, audit or legal-review reports
- infrastructure questionnaires, cost/billing analyses, architecture notes
- anything containing secrets, credentials, internal URLs, or unpublished decisions

Pushing such a file to **any** branch of this repo publishes it. Remember that a public
repo also exposes its **entire history**, so an internal file is not "safe" just because a
later commit deletes it — removing it requires history rewriting.

### Where internal documents belong

Internal documents and reports go in the **private** repository:

```
git@github.com:OwnCup/private_documents.git   (commit directly to main)
```

If you find an internal document that has been committed to this public repo by mistake:

1. Move it to `OwnCup/private_documents` (so it is not lost).
2. Remove it from this public repo **including from history** (delete the offending
   branch, or rewrite history if it reached `main`).
3. Verify no internal file remains in any ref:
   `git log --all --pretty=format: --name-only --diff-filter=A | sort -u`

## Delivery

Work on a feature branch and open a Pull Request into `main` (this repo has no `develop`).
Never push directly to `main`.
