---
target_repo: https://github.com/zaniebot/exp-3-task-test-workspace
target_ref: agent/vverziwe-plan-a-calculator-module
session: sessions/zaniebot-exp-3-task-test-workspace/ybsvwulh-implement-calculator-multiply-and-divide-modules/chat.jsonl
summary: sessions/zaniebot-exp-3-task-test-workspace/ybsvwulh-implement-calculator-multiply-and-divide-modules/summary.md
reviews:
  - reviews/ybsvwulh-implement-calculator-multiply-and-divide-modules/auto-reviewer-qpleudus.md
---

# Implement calculator multiply and divide modules

Implement the multiply and divide operations for the calculator module as described in docs/calculator-design.md.

Steps:
1. Create calculator/multiply.py with a `multiply(a, b)` function.
2. Create calculator/divide.py with a `divide(a, b)` function that raises ZeroDivisionError when b is zero.
3. Update calculator/\_\_init\_\_.py to also export multiply and divide.
4. Create tests/test_multiply.py and tests/test_divide.py with unit tests covering normal cases, edge cases, and the division-by-zero error case.
5. Ensure all tests pass.
