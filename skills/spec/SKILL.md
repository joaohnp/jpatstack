---
name: spec
description: Turn an agreed design, prototype verdict, or issue into a concise spec and, if needed, a ticket handoff. Plan the work without starting it.
---

# Spec first, tickets second

Start from what was agreed. Read the relevant issue and comments or prototype verdict; reuse a sufficient spec. Cite a prior decision rather than retelling it. If a choice changes what someone would build, ask or mark it open.

State the problem, intended behavior, how to check it, and what to leave out. Give one example that would reject a plausible wrong result: “Two reviewers rate the same message; each can read their own evaluation and neither can see the other's.” That rules out overwriting a review and exposing it. “Support feedback” rules out neither.

If one person can finish and demonstrate it in a sitting, **the spec is the ticket**; a paragraph can be enough. Otherwise split into independently verifiable outcomes, not separate code, test, and docs chores. Number the proposed tickets so the user can correct the split. For each, give **Title**, **What it delivers** (the behavior to demonstrate), and **Blocked by** (ticket numbers or “none”). Name the owning repo when work crosses repos. A blocker means the work cannot start until that ticket is done.

**Winning condition:** A builder who missed the conversation can start the right piece and show whether it works. Return the draft; publish only the requested, agreed work. A spec is not permission to implement.
