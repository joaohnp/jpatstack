---
name: follow-the-problem
description: Diagnose a wrong number, broken interaction, layout glitch, API failure, or slow request. Trace the reported case and explain the cause; fix only when asked.
---

# Follow the problem

Reproduce the reported case where the person saw it. Keep the period and filters, viewport and click, or workload and cache state fixed. Establish what should happen from the requirement or a worked example, not from the code you're investigating.

Follow that one case to the first mismatch. For a note missing after refresh, did the write store it? Did the next read return it? If the read contains the note, follow it into the screen; another write retry won't explain why it isn't displayed. Choose the cheapest observation that separates the remaining explanations. Widen the search only when an observation points off this path. A source line suggests a mechanism; a run shows whether this case hit it.

If two fixes failed on the same premise, write down what both assumed and test it before a third. For a speed claim, check that both runs did the same work and returned the right output. If the spread between runs is larger than the effect, say these runs can't distinguish it from noise.

**Winning condition:** Name the cause and show the observation that rules out the plausible alternative. Give the command or relevant output. If unresolved, name the last verified fact and the missing observation. Stop at the explanation unless a fix was requested; then replay the original case.
