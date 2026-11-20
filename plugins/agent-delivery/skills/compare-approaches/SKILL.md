---
name: compare-approaches
description: Compare viable implementation options when an architecture, dependency, or integration choice could materially affect delivery.
---

1. State the decision, hard requirements, and the tradeoff that matters most. Inspect the closest existing implementation and test before proposing alternatives.
2. Shortlist the two leading options when both are viable. Add another only if it addresses a material constraint the others miss. Eliminate any option that fails a hard requirement, then compare the survivors on compatibility, effort, operational cost, reversibility, and how well each can be verified. Separate evidence from assumptions.
3. If the ranking hinges on an assumption, run one cheap check that could reverse it. Update the ranking from the result. Stop exploring when the remaining unknowns would leave the decision unchanged. For a consequential unknown that cannot be checked, make the decision conditional and state what would resolve it.
4. Give the preferred option and the decisive tradeoff in a few lines. When implementation is in scope, turn the choice into small deliverable units with checks and start the first unit.
