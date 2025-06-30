# Variables and Data Types

:::{note}
In Python, variables are created when you assign a value to them — there's no need to declare their type explicitly.
:::

## What is a Variable?

A **variable** is a name that refers to a value stored in memory.

```python
x = 10
name = "Alice"
is_active = True
```

You can think of variables as labels for values.

## Dynamic Typing

Python uses **dynamic typing**, meaning you don't need to declare the type of a variable.

```python
value = 5        # int
value = "hello"  # now a string
value = 3.14     # now a float
```

:::{warning}
This flexibility is powerful but requires discipline to avoid bugs due to unintended type changes.
:::


## Type Checking

You can check a variable's type using `type()`:

```python
age = 25
print(type(age))  # <class 'int'>
```

## Type Casting

You can convert between types:

```python
x = "123"
x = int(x)      # now an integer
y = float("3.5")
z = str(456)
```

:::{tip}
Use `str()`, `int()`, and `float()` to convert between types.
:::

## Summary

- Python variables are dynamically typed.
- Use meaningful names for clarity.
- Learn common data types to work effectively with data.