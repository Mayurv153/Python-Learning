# 🛠️ Defining Functions in Python

The `def` keyword is the foundation of modularity in Python. It allows you to wrap sequence of statements into a single unit that can be executed whenever needed.

---

### 1. 🏗️ Basic Syntax
To define a function, use the `def` keyword followed by the function name and parentheses `()`.

```python
def greet():
    """
    This is a docstring. it explains what the function does.
    """
    print("Welcome to Python Functions!")

# Calling the function
greet()
```

### 2. 📝 Naming Conventions (PEP 8)
- Use **lowercase** with words separated by underscores (`snake_case`).
- Names should be **descriptive** (e.g., `calculate_area` instead of `ca`).
- Avoid using reserved keywords (like `list`, `str`, `def`).

### 3. 📥 Parameters and Arguments
Functions can accept inputs called **parameters**. When you call the function, you provide **arguments**.

```python
def welcome_user(name):
    print(f"Hello, {name}! Glad to have you here.")

welcome_user("Mayur") # "Mayur" is the argument
```

### 4. 📤 The `return` Statement
A function can send a result back to the caller using the `return` keyword. A function without a `return` statement returns `None` by default.

```python
def add_numbers(a, b):
    return a + b

result = add_numbers(10, 20)
print(f"The sum is: {result}")
```

### 5. 📜 Docstrings
Professional Python code always includes a **Docstring** immediately after the function header. It describes the function's purpose, parameters, and return value.

```python
def multiply(x, y):
    """
    Multiplies two numbers and returns the product.
    
    Args:
        x (int/float): The first number.
        y (int/float): The second number.
        
    Returns:
        int/float: The product of x and y.
    """
    return x * y
```

---

> [!IMPORTANT]
> **Indentation Matters:** In Python, the code block inside a function is defined by its indentation level (usually 4 spaces).

---
