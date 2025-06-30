# Control Flow

:::{note}
Control flow allows you to dictate how your Python program makes decisions and repeats actions.
:::

## Conditional Statements

### if, elif, else

You can execute different blocks of code depending on conditions.

```python
temperature = 25

if temperature > 30:
    print("It's hot outside.")
elif temperature > 20:
    print("Nice weather.")
else:
    print("It's a bit cold.")
```

Python uses indentation to define code blocks. Be consistent with spacing.

## Comparison Operators

These are used to compare values in conditions:

- `==` : equal to  
- `!=` : not equal to  
- `>`  : greater than  
- `<`  : less than  
- `>=` : greater than or equal to  
- `<=` : less than or equal to  

You can also combine conditions with:

- `and`
- `or`
- `not`

```python
age = 22
has_id = True

if age >= 18 and has_id:
    print("Access granted.")
```

## Loops

### for loop

Used to iterate over sequences like lists or ranges.

```python
for i in range(5):
    print(i)
```

### while loop

Executes while a condition is true.

```python
count = 0
while count < 3:
    print("Count:", count)
    count += 1
```

:::{warning}
Avoid infinite loops by ensuring the condition eventually becomes false.
:::

## break and continue

- break: exits the loop entirely.  
- continue: skips to the next iteration.

```python
for i in range(10):
    if i == 5:
        break
    if i % 2 == 0:
        continue
    print(i)
```

## match statement (Python 3.10+)

Alternative to multiple if/elif blocks.

```python
command = "start"

match command:
    case "start":
        print("Starting...")
    case "stop":
        print("Stopping...")
    case _:
        print("Unknown command")
```

## Summary

- Use if, elif, else for conditional branching.
- Use for and while loops for repetition.
- Use break and continue to control loop behavior.
- Use match (Python 3.10+) for clearer branching on known values.
