# Day 02: Python Basics (Quick Reference Guide) 🐍

## Exercise 1: Print a Pattern 🎨

**Concept**: Using loops to create visual patterns

```python
num = int(input("Enter a number: "))
for i in range(1, num + 1):
    print(' ' * (num-i) + '*' * (2*i - 1))
```

**What it does**:

- Takes user input for a number
- Creates a diamond/pyramid pattern with spaces and asterisks
- Each row has `(num-i)` spaces and `(2*i-1)` asterisks
- Builds upward as i increases

**Key Concepts** ✨:

- `range(1, num + 1)` - Loop from 1 to num (inclusive)
- String multiplication `' ' * n` - Repeats string n times
- `input()` - Gets user input
- `int()` - Converts string to integer

---

## Exercise 2: Multiplication Table 📊

**Concept**: Nested loops for creating tables

```python
print("Multiplication Table:")

for i in range(1, 11):
    for j in range(1, 11):
        print(f"{i * j:4}", end=' ')
    print()
```

**What it does**:

- Creates a 10×10 multiplication table
- Outer loop iterates rows (1-10)
- Inner loop iterates columns (1-10)
- Each cell shows `i * j`

**Key Concepts** 🔢:

- **Nested loops** - Loop inside a loop for 2D patterns
- **f-strings** - `f"{i * j:4}"` formats output with 4 characters width
- `end=' '` - Prints space instead of newline
- `print()` with no arguments - Moves to next row

---

## Exercise 3: DNA Nucleotide Counter 🧬

**Concept**: Counting characters in a string using conditionals

```python
DNA = "ATGCGATACGCTTGA"

countA = 0
countT = 0
countG = 0
countC = 0

for x in DNA:
    if x == 'A':
        countA += 1
    elif x == 'T':
        countT += 1
    elif x == 'G':
        countG += 1
    elif x == 'C':
        countC += 1

print("Number of A:", countA)
print("Number of T:", countT)
print("Number of G:", countG)
print("Number of C:", countC)
```

**What it does**:

- Analyzes a DNA sequence string
- Counts each nucleotide type (A, T, G, C)
- Displays the frequency of each base

**Key Concepts** 🔬:

- **For-in loop** - Iterates through each character in string
- **if-elif chains** - Tests multiple conditions
- **Counter variables** - Accumulate count with `+=`
- **String comparison** - Checks if character equals specific value

---

## Summary of Key Python Skills 📝

| Concept               | Example                  | Use Case                       |
| --------------------- | ------------------------ | ------------------------------ |
| **Input/Output**      | `input()`, `print()`     | Get user data, display results |
| **Loops**             | `for i in range()`       | Repeat actions multiple times  |
| **Nested Loops**      | Loop in loop             | Create 2D patterns/tables      |
| **String Operations** | `'*' * 5`, iterate chars | Manipulate and analyze text    |
| **Conditionals**      | `if`, `elif`, `else`     | Make decisions in code         |
| **Counters**          | `count += 1`             | Track frequencies/totals       |
| **String Formatting** | f-strings `f"{x:4}"`     | Pretty print outputs           |

---

## Quick Tips 💡

✅ Use `range(1, n+1)` to include n (range excludes end)  
✅ Chain conditions with `elif` for multiple checks  
✅ Use `for x in string` to loop through characters  
✅ `+=` is shorthand for `x = x + 1`  
✅ f-strings with `:4` format numbers/text to width  
✅ `end=' '` in print prevents newlines

---

**What You Learned**: Basic loop structures, string manipulation, pattern creation, and practical data analysis! 🚀
