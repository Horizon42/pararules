# Special Notes

- The ruleset cannot currently call functions declared after it. This means any functions that query the rules-engine cannot be compiled.
- If two things change at roughly the same time in a rule, a [[then = false]] assignment in one of them will prevent the rule from firing. Use it only when you know it will not change alongside the active tuples
