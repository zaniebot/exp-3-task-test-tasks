# Code Review: Implement calculator add and subtract modules

## What was done well

- **All 5 task steps completed**: `calculator/__init__.py`, `calculator/add.py`, `calculator/subtract.py`, `tests/test_add.py`, `tests/test_subtract.py` all created correctly.
- **Function signatures and docstrings** match the design doc exactly (`add(a: float, b: float) -> float`, etc.).
- **Good test coverage**: Tests cover positive numbers, negative numbers, mixed signs, zeros, floats, and large numbers — matching the testing strategy in the design doc.
- **Clean structure**: `tests/__init__.py` included for proper package discovery. `.gitignore` added for Python bytecode files.
- **Code is minimal and correct**: No unnecessary complexity.

## Minor observations (not blocking)

- The design doc mentions `multiply` and `divide` as future operations, but those were explicitly out of scope for this task. No issue here.
- Tests use `==` for float comparisons (e.g., `add(1.5, 2.5) == 4.0`). For these specific values this is fine since they have exact binary representations, but future tests with problematic floats should use `pytest.approx`.

## Verdict

All task requirements are fully met. The code is correct, well-structured, and the tests are thorough.

APPROVE