---
name: diagnose-failure
description: Diagnose failing tests, builds, CI runs, and unexpected application behavior, especially after a previous fix attempt failed.
---

1. Capture the failing case, expected result, and first actionable error. Read the smallest relevant log window and identify the affected entry point. Use existing logs or a regression check when they supply the same evidence as a rerun.
2. Pick the most likely cause and one plausible alternative if the evidence is ambiguous. Run the cheapest check that would distinguish them. Record the result and what it rules out. Reuse prior evidence until the code, inputs, or environment change.
3. Fix the confirmed cause in the owning layer. If the result is inconclusive, revise the hypothesis or narrow the scope before the next attempt. Repeat a command only when something changed or when checking an evidenced transient failure.
4. Rerun the original failure path or its closest reliable check. Run related tests when the fix changes shared behavior. If an external dependency prevents confirmation, state the specific blocker, what has been verified, and the evidence still needed.
