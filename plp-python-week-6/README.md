# Week 6 - Safe Functions (try / except)

## Files

- `safe_tools.py` - three functions (`safe_divide`, `safe_number`, `get_field`) that use `try` / `except` so they return a friendly message instead of crashing.
- `README.md` - this file: the assignment title, a description of each file, and the answer to the question below.

## Why can the `if` check not catch `abc` on its own?

An `if` check can only test for a problem you already know how to describe, like `b == 0`. Text such as `abc` can be wrong in many ways (letters, symbols, empty text, decimals), and it is hard to write an `if` that covers all of them. With `try` / `except`, Python just attempts `int()` and tells us when it fails, so we catch the `ValueError` without having to predict every bad input.