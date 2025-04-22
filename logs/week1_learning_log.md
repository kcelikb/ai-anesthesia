## Monday, April 21, 2025

### Topic: Reserved Words – PFEB Ch. 2 Notes

**Summary:**
- Python's reserved words (e.g., `and`, `if`, `for`, `def`, `return`) cannot be used as variable names. These keywords form the core Python vocabulary.
- While variable names are flexible, **reserved words** cannot be used as identifiers.

**Common Reserved Words:**
| Reserved Words         |
|------------------------|
| and, or, not           |
| if, else, elif         |
| for, while, break      |
| def, return, lambda    |
| import, from, as       |
| class, try, except     |

**Full List of Reserved Keywords:**
```
and       del       from      None      True
as        elif      global    nonlocal  try
assert    else      if        not       while
break     except    import    or        with
class     False     in        pass      yield
continue  finally   is        raise
def       for       lambda    return
```


---

## Tuesday, April 22, 2025

### Topic: Variable Naming Rules and Arithmetic Operators

**Summary:**
1. Variable names:
   - Cannot begin with a number.
   - Must not contain symbols.
2. Key Arithmetic Operators:
   - **Quotient Operator (`//`)**: Performs integer division.
   - **Remainder Operator (`%`)**: Returns the remainder of a division.

---

### Topic: Why `float()` is used in Python when working with `input()`

**Summary:**
- The `input()` function in Python always returns data as a string.
- Using `float()` converts the string into a floating-point number, enabling arithmetic operations.
- This is especially necessary when working with non-integer numbers like hours worked or hourly rates.
- Without conversion, attempting arithmetic operations would result in a `TypeError`.
- `int()` could also be used if only integers are expected, but `float()` is more versatile for decimals.

**Example Code:**
```python
hours = float(input('Enter hours: '))
rate = float(input('Enter rate: '))
pay = hours * rate
print(pay)
```

**Key Takeaway:**
Always explicitly convert user input to the desired numeric type (`int()` or `float()`) before performing calculations to avoid errors.