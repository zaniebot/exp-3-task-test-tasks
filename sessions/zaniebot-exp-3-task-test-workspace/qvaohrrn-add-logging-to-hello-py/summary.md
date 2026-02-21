Merge Conflict Resolution Summary

Files with conflicts: hello.py, README.md

hello.py:
- My branch added: logging module import, module-level logger, --verbose flag, 
  logging.basicConfig setup, and logger.info call in main().
- Main branch added: --name argument, personalized greeting logic, and goodbye() function.
- Resolution: Integrated both changes. main() now has both --verbose and --name flags,
  logging setup runs before the greeting, and the greeting uses the --name logic from main.
  The goodbye() function from main is preserved. The if __name__ block calls both
  main() and goodbye() as upstream intended.

README.md:
- My branch added: logging/verbose documentation.
- Main branch added: --name flag docs, goodbye() mention, and example output.
- Resolution: Combined both descriptions. The script description mentions both goodbye()
  and logging support. Kept upstream's --name docs and output examples, and added
  the --verbose documentation from my branch.