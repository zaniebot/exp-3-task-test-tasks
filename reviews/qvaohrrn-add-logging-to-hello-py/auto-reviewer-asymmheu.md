# Code Review: Add logging to hello.py

## What was done well
- **Module-level logger**: Correctly set up with `logging.getLogger(__name__)`.
- **Info message in main()**: `logger.info("main() is running")` satisfies the requirement.
- **`--verbose` flag**: Properly implemented with `argparse`, toggling between `INFO` and `DEBUG` levels.
- **Log format**: Includes timestamp, logger name, and level — a reasonable default.
- **README updated**: Documents both basic usage and the `--verbose` flag with examples.
- **Clean, minimal diff**: No unnecessary changes.

## Minor observations (non-blocking)
- `logging.basicConfig()` is called inside `main()` after argument parsing, which is fine for this use case but means any module-level log calls made at import time (before `main()`) would go to the default handler. Not an issue for this simple script.
- No explicit debug-level log message is emitted to demonstrate the `--verbose` flag in action (e.g., `logger.debug("Debug mode enabled")`). This is a nice-to-have, not a requirement.

## Verdict
All three requirements are met: module-level logger, info log in `main()`, `--verbose` flag, and README update. The code is clean and correct.

APPROVE