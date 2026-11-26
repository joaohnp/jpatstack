---
name: earn-the-diff
description: Build a requested feature or fix a bug. Trace a real case, make only the change it needs, and show the result. A feasibility question or plan is not a build request.
---

# Earn the diff

**What fails today?** Take one real input. Work out the expected result from the requirement and the underlying records. Run the unmodified path and compare. Two outcomes:

- **Already works:** report the input, expected result, and matching observation. Stop here with an empty diff. The explanation belongs in the reply, not in a new comment or test.
- **Change needed:** the observed result differs, or the requested behavior is missing. Fix that gap. If you can't tell which result is right, settle the rule first. For a reported bug, read what was already tried.

When two or more fixes that share one premise have failed the same gate, suspect the premise, not the fixes. Write down what both fixes assumed. Find an observation that would come out differently if the premise were false, and make it. Do not start the next fix before the premise is written down and tested.

Build from the data up. What does one record represent? Find where the existing path first fails the requirement. Can you remove or correct a rule there instead of compensating for it downstream?

**Subtract before you add.** Prefer the design that leaves the least code to maintain, not the fewest lines in this diff. If two callers would have to change for the same business reason, give that rule one owner. Similar-looking code alone isn't a reason to combine it. Add an abstraction only when you can show what a real caller no longer has to know or do. Leave out a flag, table, or dependency unless a present requirement fails without it. Work directly unless another agent has a specific independent job.

Verify the real thing: drive the screen, run the command, or read back the stored value. Keep a regression test for a plausible, consequential failure existing coverage misses. Extend an existing case if it suffices. Test public behavior so an internal refactor can still pass.

**Don't let the code under test supply its own answer key.** What was May's cost per win? We spent R$120 in May; three deals were won in May and a fourth in June. Expect **R$40 per win** (120 ÷ 3). A calculator that forgets the date filter returns R$30 (120 ÷ 4). If the test also calls that calculator for its expected value, it compares R$30 with R$30 and passes. Assert R$40 instead.

Watch a regression check fail for the right reason, then replay it after the fix. Run required repo checks; broaden them for a named risk.

**Winning condition:** Lead with what changed and the command or URL that shows the before/after on the original case. If no diff was needed, show the existing behavior that settles it. Say if the baseline is missing or a material risk remains unverified. Commit in focused pieces when asked; distinguish local, committed, pushed, and live. A build request alone doesn't authorize a merge, deploy, or production SQL.
