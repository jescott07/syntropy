# Working with Files

:::{note}
Python provides built-in functions to create, read, write, and manage files using the `open()` function and context managers.
:::

## Opening a File

Use the `open()` function with a file path and a mode:

- `"r"`: read (default)
- `"w"`: write (overwrite)
- `"a"`: append
- `"x"`: create new file (error if exists)
- `"b"`: binary mode
- `"t"`: text mode (default)

```python
file = open("example.txt", "r")
content = file.read()
file.close()
```

## Using a Context Manager

The recommended way is using `with`, which automatically closes the file:

```python
with open("example.txt", "r") as file:
    content = file.read()
    print(content)
```

## Reading from a File

You can read content in different ways:

```python
with open("example.txt", "r") as file:
    print(file.read())       # entire file
    print(file.readline())   # one line
    print(file.readlines())  # list of lines
```

## Writing to a File

Opening a file in `"w"` mode overwrites it:

```python
with open("output.txt", "w") as file:
    file.write("This is a new file.\n")
    file.write("Another line.\n")
```

Use `"a"` mode to append:

```python
with open("output.txt", "a") as file:
    file.write("This will be added at the end.\n")
```

## Working with File Paths

Use the `os` or `pathlib` modules to manage file paths:

```python
import os

file_path = os.path.join("data", "info.txt")
with open(file_path, "r") as file:
    print(file.read())
```

Or with `pathlib`:

```python
from pathlib import Path

file_path = Path("data") / "info.txt"
with file_path.open("r") as file:
    print(file.read())
```

## Checking File Existence

```python
import os

if os.path.exists("data.txt"):
    print("File exists.")
else:
    print("File not found.")
```

Or using `pathlib`:

```python
from pathlib import Path

if Path("data.txt").exists():
    print("File exists.")
```

## Summary

- Use `open()` with modes like `"r"`, `"w"`, `"a"` to work with files.
- Use `with` for safer and cleaner file handling.
- Use `os` or `pathlib` to manage file paths and check existence.
- Always be careful when writing files — `"w"` will overwrite them.
