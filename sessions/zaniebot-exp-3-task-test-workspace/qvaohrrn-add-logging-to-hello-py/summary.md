Added Python logging to hello.py:
- Set up a module-level logger using logging.getLogger(__name__)
- Configured logging.basicConfig in main() with timestamped format
- Added an info-level log message when main() runs
- Added a --verbose CLI flag (via argparse) that switches logging from INFO to DEBUG level
- Updated README.md to document the new --verbose flag