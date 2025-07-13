## 1.  What is Input/Output in Python?

Input means getting data from the user (keyboard).

Output means showing data to the user (usually on screen).

Python provides built-in functions for both:

input() → to get input.

print() → to show output.

## 2. Concepts of Input/Output in Python

🔹 Input: input() function

Always returns a string (text).

✅ Syntax:

```
variable = input("Enter something: ")
```
You often need to convert the input to another type like int() or float().

✅ Examples:

```
name = input("Enter your name: ")
print("Hello", name)

```

```
age = int(input("Enter your age: "))
print("You will be", age + 1, "next year")

```

🔹 Output: print() function
Displays information to the screen.

Can print text, variables, or a mix.

✅ Syntax:

```
print("Hello")  # prints text
print("Age:", 25)  # prints multiple things

```

Optional Parameters:

sep: How to separate items (default is space)

end: What to print at the end (default is newline \n)

```
print("A", "B", "C", sep="-")  # A-B-C
print("Hello", end=" ")       
print("World")  # Output: Hello World

```
🔹 Type Conversion with Input:
Since input() gives a string, we convert it when needed:

```
a = int(input("Enter number: "))  # now a is an integer
b = float(input("Enter decimal: "))  # now b is a float

```
🔹 Multi-Input:
Getting multiple values in one line using split().
```
x, y = input("Enter two numbers: ").split()
print("X:", x)
print("Y:", y)
```
You can also convert them at the same time:
```
x, y = map(int, input("Enter two numbers: ").split())
```
🔹 Formatted Output (f-strings)
Nice way to insert variables into strings:
```
name = "Alice"
age = 20
print(f"My name is {name} and I am {age} years old.")
```
## 3. Input/Output Examples

✅ Simple Examples:

```
# Example 1: Input a name and print it
name = input("Your name: ")
print("Hi", name)

# Example 2: Input a number and print it doubled
num = int(input("Enter number: "))
print("Double:", num * 2)

# Example 3: Print using sep and end
print("Python", "is", "fun", sep="-", end="!!!\n")

```

Tricky I/O-Only Examples:

```
# Tricky 1: Input as string but looks like number
data = input("Enter something: ")
print("You entered:", data)
print("As integer:", int(data))  # Fails if not numeric

# Tricky 2: Multiple inputs
a, b, c = input("Enter 3 values: ").split()
print("A:", a, "B:", b, "C:", c)

# Tricky 3: Combine input and formatted output
name = input("Enter name: ")
score = float(input("Enter score: "))
print(f"{name}'s score is {score:.2f}")

# Tricky 4: Unexpected whitespace
x = input("Enter: ")
print("With space:", x)
print("Stripped:", x.strip())  # removes leading/trailing spaces

# Tricky 5: Input but ignore part of it
_ = input("Enter something (we'll ignore it): ")
print("I ignored what you said.")
```

## 4. ✅ Tips for Mastering Python Input/Output

Tip No.	Tip
> 1️⃣	Remember: input() always returns a string
> 2️⃣	Use int(), float(), etc. to convert input
>3️⃣	Use split() and map() for multiple inputs
>4️⃣	print() is very flexible: use sep, end, and f-strings
>5️⃣	Use .strip() to remove unwanted spaces
>6️⃣	Always test user input with edge cases (empty input, non-number, etc.)
>7️⃣	When using multiple input()s, prompt clearly for each


