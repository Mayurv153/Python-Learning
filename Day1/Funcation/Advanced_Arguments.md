# 🚀 Advanced Arguments: *args and **kwargs

When you don't know the exact number of arguments your function will receive, Python provides two special tools: `*args` and `**kwargs`.

---

### 1. 📦 Non-Keyword Arguments (`*args`)
The `*args` syntax allows a function to accept any number of **positional arguments**. Inside the function, `args` is treated as a **tuple**.

```python
def sum_all(*numbers):
    total = 0
    for num in numbers:
        total += num
    return total

print(sum_all(1, 2, 3))       # Output: 6
print(sum_all(10, 20, 30, 40)) # Output: 100
```

### 2. 🏷️ Keyword Arguments (`**kwargs`)
The `**kwargs` syntax allows a function to accept any number of **keyword (named) arguments**. Inside the function, `kwargs` is treated as a **dictionary**.

```python
def display_profile(**details):
    for key, value in details.items():
        print(f"{key.capitalize()}: {value}")

display_profile(name="Mayur", role="Developer", city="Pune")
```

### 3. 🧩 Combining All Argument Types
When combining them, you must follow this specific order:
1. Positional arguments
2. Default arguments
3. `*args`
4. `**kwargs`

```python
def complex_function(a, b, *args, **kwargs):
    print(f"a: {a}, b: {b}")
    print(f"Additional positional: {args}")
    print(f"Additional keyword: {kwargs}")

complex_function(1, 2, 3, 4, 5, x=100, y=200)
```

---

> [!TIP]
> **Pro Tip:** The names `args` and `kwargs` are just conventions. You could use `*stuff` or `**data`, but sticking to `*args` and `**kwargs` is the standard practiced by professional Python developers worldwide.

---
