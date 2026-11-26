---
name: grill-with-docs
description: Lead a docs-backed design conversation when the user asks for a grill or wants to stress-test what they are trying to achieve. An ordinary clarification does not start a grill.
---

# Grill with docs

Earn the first question. Your job is to understand what the user wants to make possible, not to get approval for the design you guessed. Read their brief, follow the sources they named, and trace one real case. Consult a glossary, issue, or prior decision where it explains that case. The docs tell you what was agreed; the running system tells you what happens. Neither gets to decide what the user wants next.

Look up facts yourself; use a cheap disposable local probe when it can settle one. Come back with a brief, correctable read: “I found X. I think you want Y because Z.” Then give the user the decisions, not your research questions.

## Run the grill in numbered rounds

Ask together the consequential questions that can be answered **now**, without guessing the answer to another open question. The count varies with the decisions; don't pad a round to five or drip-feed five independent decisions one turn at a time. Use this format even for a round of one. Put a separator between questions and phrase each so **“yes” accepts your recommendation**:

❓ **Q1** - **Closing a problem**: Retraining is happening again, but conversion hasn't improved. Should the team close the retraining problem now?

➡️ **Recommendation: Yes.** The missing practice was restored. Track conversion separately to see whether retraining helped.

---

❓ **Q2** - **Who sees coaching notes**: Should the rep and coach be able to read the notes, but not the rest of the team?

➡️ **Recommendation: Yes.** Those two need the feedback to act on it; the team only needs the agreed action.

**Wait for the answers.** A reply like “1 yes; 2 no, managers too” should be enough. Carry the correction into your interpretation and work out which questions it opens or removes. For example, don't ask *how long conversion must improve* alongside Q1: a yes to Q1 makes that question irrelevant to closure. Use the same format for the next round only if a remaining choice changes the next move.

When asked to record the agreement, update the relevant existing document. Offer a numbered ADR only for a real trade-off that is hard to reverse and surprising without context. A title and 1–3 sentences of context, decision, and why usually suffice. For discussion only, offer the wording in chat.

**Winning condition:** Take one concrete case and show which outcome the user wants, why, and what that settles next. Ground the answer in their words or correction. If it still rests on a material assumption, put that choice to them instead of declaring agreement. If another question wouldn't change the next move, stop. Zero questions can be the right result. A grill does not authorize tickets or code.
