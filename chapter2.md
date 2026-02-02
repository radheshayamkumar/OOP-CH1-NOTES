# Chapter 2: Introduction to C++

---

## 1. Introduction to C++

C++ is a programming language used to write programs that can solve real-world problems efficiently. It is called a **general-purpose language** because it can be used to develop many types of software such as:

* Operating systems
* Banking applications
* Games
* Desktop software
* Embedded systems

C++ is powerful because it supports **both procedural programming and object-oriented programming**. This makes it flexible and widely used in both academia and industry.

In simple words:

> **C++ lets us write fast programs and also organize them properly.**

---

## 2. What is C++?

C++ is an **extension of the C language**. It was developed to overcome the limitations of C.

### Key Points about C++

* Developed by **Bjarne Stroustrup**
* Adds object-oriented features to C
* Supports classes, objects, inheritance, etc.
* Very fast execution
* Gives control over memory

### Why C++ Was Needed (C vs C++)

C language:

* Focuses only on functions
* Data is not well protected
* Not suitable for large software

C++:

* Focuses on **data + functions together**
* Provides data security
* Suitable for large and complex programs

---

## 3. A Simple C++ Program

Let us start with a basic C++ program.

```cpp
#include <iostream>
using namespace std;

int main() {
    cout << "Hello World";
    return 0;
}
```

---

### Explanation Line by Line

#### `#include <iostream>`

* This is a **preprocessor directive**
* It includes input-output stream library
* Required to use `cin` and `cout`

#### `using namespace std;`

* `std` stands for standard
* It avoids writing `std::cout` again and again

#### `int main()`

* `main()` is the starting point of execution
* Every C++ program must have `main()`

#### `cout << "Hello World";`

* `cout` prints output on screen
* `<<` is insertion operator

#### `return 0;`

* Ends the program
* Returns control to operating system

---

## 4. More C++ Statements

### Input Statement (`cin`)

Used to take input from the user.

```cpp
int a;
cin >> a;
```

Here:

* `cin` reads value from keyboard
* `>>` is extraction operator

---

### Output Statement (`cout`)

Used to display output.

```cpp
cout << a;
```

---

### Multiple Input and Output

```cpp
int a, b;
cin >> a >> b;
cout << a + b;
```

---

### Conditional Statement (`if`)

Used to make decisions.

```cpp
if (a > b) {
    cout << "A is greater";
}
```

---

### Loop Statement (`for`)

Used to repeat statements.

```cpp
for(int i = 1; i <= 5; i++) {
    cout << i;
}
```

---

## 5. Structure of a C++ Program

A C++ program follows a well-defined structure.

### General Structure

```cpp
#include <iostream>
using namespace std;

class Sample {
    // class definition
};

int main() {
    // program logic
    return 0;
}
```

---

### Parts of C++ Program Structure

1. **Documentation Section**

   * Comments explaining program

2. **Preprocessor Directives**

   * `#include`, `#define`

3. **Global Declarations**

   * Global variables and functions

4. **Class Definitions**

   * User-defined classes

5. **Main Function**

   * Execution starts here

6. **User Defined Functions**

   * Additional functions if required

---

## 6. Tokens, Expressions and Control Structures

---

## 6.1 Tokens in C++

A **token** is the smallest unit of a C++ program.

Example:

```cpp
int sum = a + b;
```

Tokens here are:

* `int`
* `sum`
* `=`
* `a`
* `+`
* `b`
* `;`

---

### Types of Tokens

1. Keywords
2. Identifiers
3. Constants
4. Operators
5. Special symbols

---

## 7. Keywords

Keywords are **reserved words** in C++.

They have:

* Fixed meaning
* Predefined use

### Examples

* `int`
* `float`
* `if`
* `else`
* `while`
* `return`
* `class`
* `public`
* `private`

### Important Rules

* Cannot be used as variable names
* Cannot be modified

---

## 8. Identifiers

Identifiers are names given to:

* Variables
* Functions
* Classes

### Rules for Identifiers

* Must start with letter or underscore
* Cannot start with digit
* No special symbols except `_`
* Case-sensitive

### Examples

```cpp
int totalMarks;
float average_score;
```

---

## 9. Constants

Constants are values that **do not change** during program execution.

---

### Types of Constants

#### Integer Constants

```cpp
10, -25, 0
```

#### Floating Point Constants

```cpp
3.14, -7.5
```

#### Character Constants

```cpp
'a', 'A'
```

#### String Constants

```cpp
"Hello"
```

---

## 10. C++ Data Types

Data types specify **what type of data** a variable can store.

---

### 10.1 Basic Data Types

| Data Type | Description      |
| --------- | ---------------- |
| int       | Integer values   |
| float     | Decimal values   |
| double    | Large decimals   |
| char      | Single character |
| bool      | true or false    |

---

### 10.2 Derived Data Types

* Arrays
* Pointers
* References
* Functions

---

### 10.3 User Defined Data Types

* struct
* union
* enum
* class

---

## 11. Variables

A **variable** is a named memory location that stores data.

---

### Declaration of Variables

```cpp
int age;
float salary;
char grade;
```

---

### Initialization of Variables

```cpp
int x = 10;
```

---

## 12. Dynamic Initialization of Variables

Dynamic initialization means assigning values to variables **during runtime**.

### Example

```cpp
int a, b;
cin >> a >> b;
int sum = a + b;
```

Here:

* `sum` is initialized using runtime values

### Advantage

* Flexible
* Useful for real-time programs

---

## 13. Reference Variables

A **reference variable** is another name for an existing variable.

---

### Syntax

```cpp
int x = 10;
int &ref = x;
```

Here:

* `ref` refers to `x`
* Both point to same memory

---

### Example

```cpp
int a = 5;
int &b = a;
b = 20;
cout << a;
```

Output:

```
20
```

---

### Advantages of Reference Variables

* No extra memory
* Faster than pointers
* Used in function calls

---

## Conclusion

C++ is a powerful language that:

* Supports structured and object-oriented programming
* Provides control, speed, and flexibility
* Is the foundation for advanced OOP concepts

Understanding this chapter properly is **mandatory** before learning classes, objects, and inheritance.

---
