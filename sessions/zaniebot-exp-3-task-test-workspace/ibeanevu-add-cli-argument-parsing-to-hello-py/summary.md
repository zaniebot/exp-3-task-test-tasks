Merge Conflict Resolution Summary
==================================

There was one conflict in README.md between the feature branch and main:

- Feature branch (HEAD): Added documentation for the new --name CLI flag usage.
- Main branch: Had default output examples showing "Hello from the task queue!" and "Goodbye from the task queue!".

Resolution: Kept both sections — the default output documentation from main comes first, followed by the --name flag usage documentation from the feature branch. This gives users complete information about both default behavior and the new CLI option.

Additionally, updated test_hello.py to:
1. Patch sys.argv in existing tests so argparse doesn't fail when run under pytest.
2. Added a new test (test_main_with_name) to verify the --name flag works correctly.

No other files had conflicts. hello.py (with argparse) was cleanly merged.