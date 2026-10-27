| Bug | Observed Problem | Root Cause | Fix Applied |
|---|---|---|---|
| Average calculation | Returned 135.0 instead of 90.0; single mark caused an error | Dividing by `len(marks) - 1` | Changed the denominator to `len(marks)` |
| Pass boundary | Mark 40 returned `False` | Used `>` instead of `>=` | Changed the condition to `mark >= PASS_MARK` |
| Distinction grade | Mark 95 returned `First` | Checked `>= 60` before `>= 90` | Checked the Distinction condition first |

## Testing Summary

- **RED:** Tests failed with the buggy implementation.
- **FIX:** Corrected the average calculation, passing boundary, and grade-condition order.
- **GREEN:** All 9 tests passed after the fixes.

## Conclusion

The bugs were identified through unit testing and corrected by applying the RED → FIX → GREEN cycle.
