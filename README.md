# PLP Python Week 6 Assignment

## Files

- `safe_tools.py`: three functions that handle errors without crashing:
  `safe_divide` handles division by zero, `safe_number` handles text that
  is not a number, and `get_field` handles a missing dictionary key.

## Why can the `if` check not catch "abc" on its own?

An `if` check can only test for cases I thought of in advance, so it will
always have gaps. For example, `text.isdigit()` rejects "-5", which `int()`
accepts. The only reliable way to know whether text can become a number is
to attempt the conversion and handle the failure, and `try` / `except` lets
Python itself decide what is valid.

## Author

Loise