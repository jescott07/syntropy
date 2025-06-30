# Functions

:::{note}
Functions allow you to reuse blocks of code by encapsulating them under a single name. This makes your programs more modular, readable, and maintainable.
:::

## Defining a Function

A function is defined using the `def` keyword, followed by its name and parentheses.

```python
def greet():
    print("Hello!")
```

To call the function:

```python
greet()
```

## Parameters and Arguments

Functions can receive inputs, called parameters.

```python
def greet(name):
    print(f"Hello, {name}!")
```

```python
greet("Maria")
```

You can define multiple parameters:

```python
def add(a, b):
    return a + b

result = add(
