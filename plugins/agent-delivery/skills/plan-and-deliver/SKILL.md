---
name: plan-and-deliver
description: Plan, implement, and verify a feature or multi-step engineering change with focused investigation and small work units.
---

1. Define the deliverable, observable acceptance checks, and constraints. Plan before editing. For a small, clear change, use one line. For larger work, list ordered units with a concrete result and check for each. Make a single pass through the relevant entry point, repository guidance, and nearest tests before filling in details.
2. Identify the uncertainty most likely to change the plan. Start with the existing repo pattern. If another approach is viable and the choice matters, compare the leading options against correctness, scope, maintenance cost, and verification effort. Probe the cheapest decisive unknown with a targeted read, test, or spike. Choose the simplest evidenced approach that meets the acceptance checks and record why in one sentence.
3. Complete one unit at a time through the normal entry point. Batch independent reads and request narrow tool output. Keep a short record of commands, results, and decisions only when it prevents repeat work. If a check fails, isolate the earliest actionable error and retry only when there is a new hypothesis or a changed condition.
4. Verify each acceptance check with the smallest meaningful test, then run broader checks when the repo requires them or the change crosses shared boundaries. Review the diff for unintended scope. Report what shipped, what passed, and any unresolved assumption or gap. Stop once the acceptance checks are met and required verification is complete.
