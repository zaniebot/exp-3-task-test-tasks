Implemented multiply and divide operations for the calculator module:

1. Created calculator/multiply.py with a `multiply(a, b)` function that returns `a * b`.
2. Created calculator/divide.py with a `divide(a, b)` function that returns `a / b` and raises `ZeroDivisionError` when `b` is zero.
3. Updated calculator/__init__.py to also export `multiply` and `divide`.
4. Created tests/test_multiply.py (7 tests) covering positive/negative numbers, mixed signs, zero, one, floats, and large numbers.
5. Created tests/test_divide.py (9 tests) covering positive/negative numbers, mixed signs, zero numerator, division by one, floats, large numbers, division by zero, and zero divided by zero.
6. All 28 tests pass (including the pre-existing add and subtract tests).