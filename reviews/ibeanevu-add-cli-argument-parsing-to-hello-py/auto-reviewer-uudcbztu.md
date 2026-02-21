# Code Review: Add CLI argument parsing to hello.py

## What was done well
- Correctly uses `argparse` from the standard library — no extra dependencies needed.
- Preserves the original default behavior (`"Hello from the task queue!"`) when `--name` is not provided.
- Clean, readable code with proper `main()` function structure.
- README updated with clear usage example showing the `--name` flag.
- Commit is atomic and well-described.

## Minor observations
- `--name ""` (empty string) would fall through to the default message due to the `if args.name:` truthiness check, which is arguably reasonable behavior rather than a bug.
- No issues with the implementation — `argparse`, argument definition, and conditional output are all correct.

## Verdict

The task asked for three things: (1) add argparse, (2) accept `--name` flag printing `Hello, <name>!`, (3) update README. All three are done correctly and cleanly.

APPROVE