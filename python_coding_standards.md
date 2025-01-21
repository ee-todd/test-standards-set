# Python Coding Standards

## 1. Naming Conventions
- Follow PEP 8 guidelines for naming:
  - Variables and functions: snake_case
  - Classes: PascalCase
  - Constants: UPPERCASE_WITH_UNDERSCORES
- Avoid single-character variable names except for counters or iterators (e.g., `i`, `j`).

## 2. Code Layout
- Use 4 spaces per indentation level.
- Limit lines to 79 characters.
- Surround top-level function and class definitions with two blank lines.
- Use one blank line to separate methods within a class.

## 3. Imports
- Use absolute imports whenever possible.
- Group imports in the following order:
  1. Standard library imports
  2. Related third-party imports
  3. Local application/library imports
- Separate each group with a blank line.

## 4. Strings
- Use single quotes (`'`) or double quotes (`"`) consistently within a project.
- Prefer f-strings for formatting over `format()` or `%`.

## 5. Exceptions
- Use specific exception classes rather than a generic `Exception`.
- Always include relevant information in exception messages.
- Use `try`...`except` blocks sparingly and avoid nesting them deeply.

## 6. Typing
- Use type hints for function arguments and return values.
```python
from typing import List

def add_numbers(a: int, b: int) -> int:
    return a + b
```

## 7. Documentation
- Write docstrings for all public modules, classes, and functions.
- Follow the Google or NumPy style for docstrings.

## 8. Testing
- Use `pytest` or `unittest` for writing and running tests.
- Structure tests in separate directories, e.g., `tests/`.
- Name test files starting with `test_`.

## 9. Code Style
- Use tools like `flake8` or `pylint` to enforce coding standards.
- Use `black` for consistent code formatting.
- Avoid using wildcard imports (e.g., `from module import *`).

## 10. Performance
- Use built-in functions and libraries whenever possible (e.g., `sum()`, `len()`).
- Avoid unnecessary list comprehensions when a generator is sufficient.

## 11. Virtual Environments
- Use `venv` or `virtualenv` for managing dependencies.
- Include a `requirements.txt` or `pyproject.toml` file for dependency tracking.

## 12. Version Control
- Exclude `.pyc` and other temporary files using `.gitignore`.
- Commit changes with meaningful messages, describing the purpose of the change.
