# Python Course

This repository contains notes and examples created while following [this YouTube playlist](https://www.youtube.com/playlist?list=PLsjpRo2EZP1Ja-GuGvkiPqmE3RGYP4lnI). The [linked video](https://www.youtube.com/watch?v=a8KDQj9ULAE&list=PLsjpRo2EZP1Ja-GuGvkiPqmE3RGYP4lnI&index=2) is the current reference.

## Run the examples

Install Python 3, open a terminal in this repository, and run:

```sh
python3 --version
python3 helloWorld.py
python3 variableTypes.py
```

On Windows, use `py` instead of `python3`. `helloWorld.py` prints two lines. `variableTypes.py` contains commented examples and naming notes, so it prints nothing until you uncomment an example and its `print(...)` line.

## Debug an error

1. Read the last line of the error message to identify the error type, then look at the file and line number shown above it.
2. Fix that line and run the same command again. Check spelling and capitalization for a `NameError`, and punctuation or indentation for a `SyntaxError` or `IndentationError`.
3. To step through a file, run `python3 -m pdb helloWorld.py` (or `py -m pdb helloWorld.py` on Windows). In the debugger, enter `n` to run the next line, `p variable_name` to inspect a variable, and `q` to quit.

If the terminal says Python is not found, install Python 3 and make sure it is available on your `PATH`. If it says the file is not found, open the terminal in this repository and check the filename.

## Variable naming

- Start a variable name with a letter or underscore, not a digit. Digits are allowed after the first character.
- Use meaningful, lowercase names with underscores between words, such as `is_active_user`.
- Use only letters, digits, and underscores. Python keywords such as `class` cannot be variable names.
- Names are case-sensitive: `user_count` and `User_Count` refer to different names.
- Avoid built-in names such as `list`, `str`, and `sum`.
- Use leading or trailing underscores only when a Python naming convention calls for them.

See [variableTypes.py](variableTypes.py) for variable examples and the naming rules.
