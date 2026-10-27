## Objective
The objective of this assignment is to identify and fix bugs in a Python script using unit testing and the RED → FIX → GREEN cycle.

## Files
- `student_utils.py` — Contains utility functions for calculating averages, checking passing marks, and assigning grades.
- `test_student_utils.py` — Contains unit tests to verify the functions.

## Bugs Identified and Fixed
1. **Average calculation:** Corrected the denominator from `len(marks) - 1` to `len(marks)`.
2. **Pass boundary:** Changed the comparison from `>` to `>=` so that a mark equal to `PASS_MARK` counts as passing.
3. **Grade assignment:** Moved the Distinction condition before the First condition to ensure marks of 90 or above receive Distinction.

## Testing Process
- **RED:** Ran the tests against the buggy code and observed failures.
- **FIX:** Corrected the identified bugs.
- **GREEN:** Reran the tests to verify the fixes.

## Expected Result
All 9 unit tests pass after the fixes.

## Conclusion
Unit testing helped identify incorrect calculations and boundary conditions. The RED → FIX → GREEN cycle verified that the corrected functions behave as expected.# nisha_25bcon1918
