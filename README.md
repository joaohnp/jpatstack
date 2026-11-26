# jpatstack

**Go deeper on the problem, not wider on the task.** Start with what the user needs to be true, follow one real case, and choose the simplest complete answer the evidence supports. Sometimes the answer is one line of code. Sometimes it's a decision and no code at all.

Ask normally. A question gets an answer; a review gets a judgment; neither starts a build. Use **grill-with-docs** deliberately when you want someone to think through a design with you.

## Install

From the project where you want to use the skills, run:

```sh
npx skills add joaohnp/jpatstack
```

Choose the skills and agent in the installer. It reads them from GitHub, so while the repository is private you'll need Git access to `joaohnp/jpatstack`.

To install just `earn-the-diff` for pi in the current project:

```sh
npx skills add joaohnp/jpatstack --skill earn-the-diff -a pi
```

Add `-g` to install across projects instead. Start pi or run `/reload` in an open session to pick up the skills.

To try a local checkout **without installing**, start pi in your working project with `pi --skill /absolute/path/to/jpatstack/skills` (or `pi --skill ./skills` from this checkout). That only affects the current session.

## Use the skills

For example: “Grill me about this design; here's the existing proposal.” In pi you can also select `/skill:grill-with-docs`. For everything else, say what you want:

| Ask | Handoff |
| --- | --- |
| [Grill me about this, with the docs](skills/grill-with-docs/SKILL.md) | An informed interpretation, the decisions that still matter, and a note or ADR when worth recording. |
| [Let me try it locally](skills/prototype/SKILL.md) | A running preview that belongs in the app. For a new layout, try A/B/C and recommend one based on the interaction. |
| [Why does the card disagree with the report?](skills/follow-the-problem/SKILL.md) | `follow-the-problem` traces one case to the first mismatch and shows the evidence for the cause. |
| [Turn this into a spec and tickets](skills/spec/SKILL.md) | If it fits one sitting, the spec is the ticket. For a split, show what each ticket delivers and what blocks it. |
| [Build the agreed change](skills/earn-the-diff/SKILL.md) | `earn-the-diff` shows the change working, or shows why the existing behavior needs no change. |
| [Review this / show me the proof](skills/review/SKILL.md) | A verdict, or direct evidence for one claim. Check related behavior when it matters. |
| [Why do I keep correcting this?](skills/retro/SKILL.md) | A proposed change where the repeat mistake originates. |

## Make it the default in a project

Loading the stack lets pi discover seven skills; it doesn't load this README as instructions. For the same approach on ordinary turns, add this working agreement once to the project's `AGENTS.md` (or the host's equivalent). No slash command or upstream plugin is required.

> Start with what I need to be true. Trace a real case when the answer depends on behavior. Test a choice you can settle by observation; ask me about decisions the evidence can't settle. If the evidence contradicts my suggestion, say so. If the existing path works, show me. When I ask for a change, fix the rule where it first goes wrong. Favor less to maintain over fewer lines in today's diff. A new layer, test, ticket, or agent needs a present reason. Lead with the result and the observation that supports it. Distinguish what you saw from what you infer. When corrected, change course. Stop at the requested handoff.

[Catalogue for review](docs/jpatstack-catalogue.md) · [Upstream comparison](docs/agent-workflow-comparison.md) · [Third-party credits and notices](THIRD-PARTY-NOTICES.md)
