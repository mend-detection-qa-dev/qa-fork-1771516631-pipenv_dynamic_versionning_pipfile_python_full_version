# Pipenv Test Case 4: Pipfile with python_full_version

## What This Tests
Tests detection of Python version from Pipfile using the `python_full_version` field (X.Y.Z format).

## Expected
3.9.18 found through PipfilePythonFullVersion

## Files
- `Pipfile` - Contains `python_full_version = "3.9.18"` in requires section

## Expected Behavior
Your version detection tool should detect **Python 3.9.18** from Pipfile.

## Priority
This is the **third priority** detection method for Pipenv projects. When both `python_version` and `python_full_version` are present, `python_full_version` takes precedence.

## Note
The `python_full_version` field provides exact versions including the patch number (e.g., "3.9.18").
