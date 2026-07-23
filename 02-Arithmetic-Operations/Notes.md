# 02 - Arithmetic Operations in Java

## Aim

To perform basic arithmetic operations on two integer variables using Java and display the results using `printf()`.

---

# Learning Objectives

After completing this program, I should be able to:

- Declare integer variables.
- Perform basic arithmetic operations.
- Understand arithmetic operators.
- Use `printf()` for formatted output.
- Understand `%d` and `%n`.
- Differentiate between `println()` and `printf()`.

---

# Why printf() instead of println()?

Java provides multiple ways to display output.

The two most commonly used methods are:

- `System.out.println()`
- `System.out.printf()`

## println()

`println()` prints the given text and automatically moves the cursor to the next line.

Example:

```java
System.out.println("Addition = " + (a + b));
```

Output:

```
Addition = 15
```

It is simple, easy to understand, and is commonly used by beginners.

---

## printf()

`printf()` prints formatted output using **format specifiers**.

Example:

```java
System.out.printf("Addition : %d%n", a + b);
```

Output:

```
Addition : 15
```

Here,

- `%d` prints an integer.
- `%n` moves the cursor to the next line.

`printf()` is preferred when we want neat, aligned, and professional-looking output.

---

## Why is printf() used in this program?

This program uses `printf()` to introduce formatted output and format specifiers.

Although the same output can be printed using `println()`, `printf()` gives better control over how the output is displayed.

---

# Program Concept

The program stores two integer values and performs the following arithmetic operations:

- Addition (`+`)
- Subtraction (`-`)
- Multiplication (`*`)
- Division (`/`)
- Modulus (`%`)

The result of each operation is displayed using `printf()`.

---

# Variables

Variables are named memory locations used to store data.

Example:

```java
int a = 10;
int b = 5;
```

- `int` → Data type
- `a`, `b` → Variable names
- `10`, `5` → Stored values

Memory Representation:

```
a → 10
b → 5
```

---

# Arithmetic Operators

| Operator | Meaning | Example |
|----------|---------|---------|
| + | Addition | a + b |
| - | Subtraction | a - b |
| * | Multiplication | a * b |
| / | Division | a / b |
| % | Modulus (Remainder) | a % b |

---

# printf() Syntax

```java
System.out.printf("format", values);
```

Example:

```java
System.out.printf("Addition : %d%n", a + b);
```

---

# Format Specifiers

## %d

Prints an integer value.

Example:

```java
System.out.printf("%d", 25);
```

Output:

```
25
```

---

## %n

Prints a new line.

It is preferred over `\n` when using `printf()` because it automatically uses the correct line separator for the operating system.

---

# Expressions

An expression combines variables and operators to produce a value.

Examples:

```java
a + b
a - b
a * b
a / b
a % b
```

---

# Integer Division

When both operands are integers, Java performs **integer division**.

Example:

```java
10 / 5 = 2
```

But,

```java
10 / 3
```

Output:

```
3
```

The decimal part is discarded.

---

# Modulus Operator (%)

The modulus operator returns the remainder after division.

Example:

```java
10 % 3
```

Output:

```
1
```

Because,

```
10 = (3 × 3) + 1
```

---

# Coding Style

Write code with proper spacing for better readability.

Preferred:

```java
int a = 10;
int b = 5;

a + b
```

Avoid:

```java
int a=10;
int b=5;

a+b
```

---

# Common Mistakes

- Forgetting the semicolon (`;`)
- Using `%d` for non-integer values
- Forgetting to provide a value for `%d`
- Using the wrong arithmetic operator
- Dividing by zero
- Forgetting `%n` when using `printf()`

---

# Viva Questions

### What is an arithmetic operator?

An arithmetic operator performs mathematical operations on operands.

---

### What is the difference between `/` and `%`?

`/` returns the quotient.

`%` returns the remainder.

---

### What is `%d`?

It is a format specifier used to print integer values.

---

### What is `%n`?

It prints a new line when using `printf()`.

---

### Difference between `println()` and `printf()`?

`println()` prints text followed by a new line.

`printf()` prints formatted output using format specifiers.

---

# Key Points to Remember

- Variables store data.
- Arithmetic operators perform calculations.
- `%d` prints integers.
- `%n` prints a new line.
- `/` performs division.
- `%` returns the remainder.
- `printf()` is used for formatted output.

---

# Quick Revision (30 Seconds)

✅ Variables store values.

✅ Arithmetic operators:

```
+   -   *   /   %
```

✅ `%d` → Integer

✅ `%n` → New line

✅ `/` → Quotient

✅ `%` → Remainder

✅ `printf()` → Formatted output

✅ `println()` → Simple output with automatic new line