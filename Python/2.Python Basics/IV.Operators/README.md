## 1. What are Python Operators?
Operators are symbols or keywords used to perform operations on variables or values.

Example:
```
a = 10
b = 3
print(a + b)  # '+' is an operator
```
## 2.  All Types of Operators in Python (with Concepts)
There are 7 main types of operators in Python:

🔹 1. Arithmetic Operators
Used for math operations.

| Operator | Meaning        | Example (`a = 10`, `b = 3`) | Result  |
| -------- | -------------- | --------------------------- | ------- |
| `+`      | Addition       | `a + b`                     | `13`    |
| `-`      | Subtraction    | `a - b`                     | `7`     |
| `*`      | Multiplication | `a * b`                     | `30`    |
| `/`      | Division       | `a / b`                     | `3.333` |
| `//`     | Floor Division | `a // b`                    | `3`     |
| `%`      | Modulus        | `a % b`                     | `1`     |
| `**`     | Exponentiation | `a ** b`                    | `1000`  |

🔹 2. Comparison (Relational) Operators
Used to compare two values. Result is True or False.

| Operator | Meaning          | Example (`a = 10`, `b = 3`) | Result  |
| -------- | ---------------- | --------------------------- | ------- |
| `==`     | Equal to         | `a == b`                    | `False` |
| `!=`     | Not equal to     | `a != b`                    | `True`  |
| `>`      | Greater than     | `a > b`                     | `True`  |
| `<`      | Less than        | `a < b`                     | `False` |
| `>=`     | Greater or equal | `a >= b`                    | `True`  |
| `<=`     | Less or equal    | `a <= b`                    | `False` |

🔹 3. Assignment Operators
Used to assign values to variables.

| Operator | Meaning                 | Example            |
| -------- | ----------------------- | ------------------ |
| `=`      | Assign                  | `x = 5`            |
| `+=`     | Add and assign          | `x += 3` (x = x+3) |
| `-=`     | Subtract and assign     | `x -= 2`           |
| `*=`     | Multiply and assign     | `x *= 4`           |
| `/=`     | Divide and assign       | `x /= 2`           |
| `//=`    | Floor divide and assign | `x //= 2`          |
| `%=`     | Modulus and assign      | `x %= 3`           |
| `**=`    | Power and assign        | `x **= 2`          |

🔹 4. Logical Operators
Used to combine multiple conditions (returns True or False).

| Operator | Meaning     | Example (`a = 5`, `b = 3`) | Result |     |     |
| -------- | ----------- | -------------------------- | ------ | --- | --- |
| `&`      | Bitwise AND | `a & b`                    | `1`    |     |     |
| \`       | \`          | Bitwise OR                 | \`a    | b\` | `7` |
| `^`      | Bitwise XOR | `a ^ b`                    | `6`    |     |     |
| `~`      | Bitwise NOT | `~a`                       | `-6`   |     |     |
| `<<`     | Left shift  | `a << 1`                   | `10`   |     |     |
| `>>`     | Right shift | `a >> 1`                   | `2`    |     |     |

🔹 6. Identity Operators
Check whether two variables refer to the same memory location.

| Operator | Meaning              | Example      |
| -------- | -------------------- | ------------ |
| `is`     | Same object?         | `a is b`     |
| `is not` | Not the same object? | `a is not b` |

🔹 7. Membership Operators
Check if a value is inside a container (like list, string).

| Operator | Meaning         | Example            |
| -------- | --------------- | ------------------ |
| `in`     | Exists?         | `'a' in 'abc'`     |
| `not in` | Does not exist? | `'z' not in 'abc'` |

3. Examples Only Based on Operators
✅ Simple Examples

```
# Arithmetic
print(10 + 2)       # 12
print(10 ** 2)      # 100

# Comparison
print(5 > 3)        # True
print(7 != 7)       # False

# Assignment
x = 5
x += 2
print(x)            # 7

# Logical
a = 10
b = 5
print(a > 5 and b < 10)  # True

# Bitwise
print(5 & 3)        # 1

# Identity
a = [1, 2]
b = a
print(a is b)       # True

# Membership
print('x' in 'text')  # True
```
Tricky Operator Examples
```
# Tricky 1: Floor division vs normal division
print(7 / 2)     # 3.5
print(7 // 2)    # 3

# Tricky 2: Negative bitwise NOT
print(~5)        # -6

# Tricky 3: Combining operators
x = 5
x *= 2 + 3       # x = x * (2 + 3)
print(x)         # 25

# Tricky 4: Logical with comparison
print(3 > 2 > 1)   # True (chained comparison)

# Tricky 5: Identity confusion
a = [1, 2]
b = [1, 2]
print(a == b)    # True (values equal)
print(a is b)    # False (different objects)
```

## 4. ✅ Tips to Master Python Operators

| Tip No. | Tip                                                                      |
| ------- | ------------------------------------------------------------------------ |
| 1️⃣     | Don’t confuse `/` and `//`. First gives float, second gives integer.     |
| 2️⃣     | Use `==` for value comparison, `is` for object identity.                 |
| 3️⃣     | Remember `input()` gives string → converting before operators is needed. |
| 4️⃣     | Know operator precedence: `*` happens before `+`, just like in math.     |
| 5️⃣     | Use parentheses `()` to make order clear.                                |
| 6️⃣     | For `and`, `or`, `not`: treat conditions as `True`/`False`.              |
| 7️⃣     | Use `in` to easily check if an item exists in a string or list.          |
