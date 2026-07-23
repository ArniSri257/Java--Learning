# ☕ 01 - Hello World

## Program

```java
public class Hello {

    public static void main(String[] args) {

        System.out.println("Hello Java");

    }
}
```

---

# Objective

- Learn the basic structure of a Java program.
- Understand every keyword used in the first program.
- Print output on the console.

---

# Program Structure

```
Java Program
│
├── Class
│      │
│      └── main() Method
│              │
│              └── Statements
```

---

# Keyword Analysis

## 1. public

- Access Modifier.
- Makes the class or method accessible from other classes.
- Think of it as a **public room** that anyone can enter.

---

## 2. class

- A blueprint used to create objects.
- Every Java program is written inside a class.

Example

```java
public class Hello
```

`Hello` is the class name.

---

## 3. Hello

- User-defined class name.
- Can be anything meaningful.
- File name **must** match the public class name.

Example

```
Hello.java
```

```
public class Hello
```

---

## 4. {

Opening curly brace.

Marks the beginning of a block.

Every opening `{` must have a matching `}`.

---

## 5. public static void main(String[] args)

This is the entry point of every Java application.

Java starts executing the program from here.

---

### public

Allows Java to access the main method.

---

### static

Allows Java to call the method without creating an object.

(Detailed understanding comes later with OOP.)

---

### void

Means the method returns nothing.

---

### main

Special method where Java begins execution.

Without `main()`, Java doesn't know where to start.

---

### String[] args

Stores command-line arguments.

Example

```
java Hello Arni 19 India
```

Then,

```
args[0] = "Arni"

args[1] = "19"

args[2] = "India"
```

`args` is just a variable name.

These are also valid:

```java
String arguments[]

String[] abc

String data[]
```

---

# System.out.println()

```
System
   │
   └── out
          │
          └── println()
```

---

## System

- Built-in Java class.
- Used to interact with the system.

---

## out

- Standard Output Stream.
- Represents the console.

---

## println()

Prints the text and moves the cursor to the next line.

---

## print()

Prints text without moving to the next line.

Example

```java
System.out.print("Hello");
System.out.print("Java");
```

Output

```
HelloJava
```

---

## println()

```java
System.out.println("Hello");
System.out.println("Java");
```

Output

```
Hello
Java
```

---

# Double Quotes ""

Anything inside double quotes is treated as a String (text).

Example

```java
"Hello"

"My name is Arni"
```

---

# Semicolon ;

Marks the end of a Java statement.

Almost every Java statement ends with `;`

---

# Important Points

- Java is Case Sensitive.
- `Hello` and `hello` are different.
- Class name and filename must be identical.
- Every Java application starts from `main()`.
- Every statement ends with `;`
- Curly braces define blocks.

---

# Things Teachers Usually Don't Tell You

- `java.lang.*` is imported automatically.
- Writing `import java.lang.*;` is optional.
- `"Hello"` is actually a String object.
- `String` is a class.
- `System` is a class.
- `println()` is a method.
- `args` is just a variable name.
- `String[] args` and `String args[]` are both valid.
- Java first compiles the program into **Bytecode (.class)** before execution.

---

# Common Mistakes

❌

```java
java Hello.java
```

✔

```java
java Hello
```

---

❌

Filename

```
hello.java
```

Class

```java
public class Hello
```

✔

```
Hello.java
```

---

❌ Missing semicolon

```java
System.out.println("Hello")
```

✔

```java
System.out.println("Hello");
```

---

❌ Missing braces `{}`

Always ensure every opening brace has a closing brace.

---

# 30 Second Revision

- Every Java program is inside a class.
- Execution starts from `main()`.
- `public` → Accessible.
- `static` → No object required.
- `void` → Returns nothing.
- `String[] args` → Stores command-line arguments.
- `System` → Built-in class.
- `out` → Console output stream.
- `println()` → Prints and moves to next line.
- `print()` → Prints on the same line.
- `java.lang` is automatically imported.

---

# Viva Questions

### Q1. Why is `main()` required?

Because Java starts executing every application from the `main()` method.

---

### Q2. What is the difference between `print()` and `println()`?

`print()` keeps the cursor on the same line.

`println()` moves the cursor to the next line.

---

### Q3. Can we change `args` to another name?

Yes.

Example

```java
String[] data
```

---

### Q4. Is `import java.lang.*;` compulsory?

No.

Java imports it automatically.

---

### Q5. What happens after compilation?

```
Hello.java
      │
      ▼
 javac Hello.java
      │
      ▼
 Hello.class (Bytecode)
      │
      ▼
 JVM
      │
      ▼
 Output
```