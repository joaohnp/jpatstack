---
name: prototype
description: Build a locally runnable preview to try an interaction, see a feature in the existing app, or compare genuinely new layouts. Stop at the design decision.
---

# Prototype

“You own the design decision, not the code. The prototype is a throwaway instrument.”. What will someone do with it that they can't settle by reading the proposal?

- **Continuity:** Build one version where the feature belongs. Reuse the neighboring screen's components, spacing, and navigation. For a state change, let the user perform the action and see the resulting state.
- **New direction:** When choosing a layout is the question, put A/B/C on one local page with a switcher. Use identical content and genuinely different ways to do the same task, not three color schemes.

Fake only what the decision doesn't depend on. Mock records can settle layout; a disputed metric needs the real calculation and matching inputs. Keep writes disposable. Skip production plumbing and permanent tests.

Open the preview and drive the deciding interaction. For alternatives, try the same task in each. Show what you observed: screenshots for a visual difference, output or timing for a behavioral one. Name the trade-off and recommend the option the evidence favors. If you didn't run it, say so rather than treating a prediction as a result.

**Winning condition:** The user can open the URL or file, try the decision for themselves, and tell what was faked. Give the restart command if needed. Stop for their verdict; a preview is not a rollout.
