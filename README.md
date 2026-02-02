# Chapter 1: Object Oriented Programming using C++

---

## 1. Introduction to Object Oriented Programming (OOP)

Programming is the process of writing instructions that tell a computer what to do. Initially, programs were small and handled simple tasks like calculations or file operations. For such programs, traditional programming methods were sufficient.

However, as software started solving **real-world problems** like banking systems, railway reservations, hospital management, and social media platforms, programs became:

* Very large
* Very complex
* Difficult to maintain
* Error-prone

This led to the need for a **better programming approach**.

### What is Object Oriented Programming?

**Object Oriented Programming (OOP)** is a programming approach where software is designed by modeling **real-world entities** using:

* **Objects** (real things)
* **Classes** (blueprints of objects)

In OOP, a program is not just a collection of functions. Instead, it is a collection of **objects that interact with each other**.

### Real-World Example

Consider a **Student**:

* Properties: roll number, name, marks
* Actions: study(), giveExam(), result()

In OOP, we convert this real-world student into a software object.

### Why OOP is Important

* Matches real-world thinking
* Organizes large programs easily
* Protects data from misuse
* Makes programs reusable and scalable

C++ is an object-oriented language that provides full support for OOP concepts.

---

## 2. Software Evolution

### Meaning of Software Evolution

**Software evolution** refers to the gradual improvement of programming techniques and languages over time to handle increasing complexity and user demands.

As problems became bigger, programming styles also evolved.

---

### Stages of Software Evolution

#### 1. Machine Language

* Uses only binary digits (0 and 1)
* Very fast execution
* Extremely difficult to write
* Error detection is almost impossible
* Machine dependent

Example:

```
10101010 11001010
```

👉 Not suitable for humans.

---

#### 2. Assembly Language

* Uses symbolic instructions (ADD, MOV)
* Slightly easier than machine language
* Requires an assembler
* Still machine dependent

Example:

```
ADD A, B
```

👉 Still complex and hardware specific.

---

#### 3. Procedure Oriented Programming (POP)

* Program divided into functions
* Focus on *how* to solve the problem
* Data is shared among functions
* Example language: C

👉 Suitable only for small programs.

---

#### 4. Object Oriented Programming (OOP)

* Program divided into objects
* Focus on *what* the problem represents
* Data and functions are combined
* Example languages: C++, Java, Python

👉 Best for large and complex software.

---

### Why POP Was Not Enough

* No proper data security
* Poor code reuse
* Difficult maintenance
* No real-world representation

OOP was introduced to overcome these issues.

---

## 3. Procedure Oriented Programming (POP)

### What is POP?

Procedure Oriented Programming is a programming approach where:

* The program is organized around **functions**
* Data is separate from functions
* Functions operate on shared data

The main focus is on **procedures (logic)**, not on data.

---

### Characteristics of POP

* Top-down programming approach
* Global data access
* Functions can modify data freely
* No data protection
* Difficult debugging for large programs

---

### POP Example

```c
int balance;

void deposit() {
    balance += 100;
}

void withdraw() {
    balance -= 50;
}
```

### What’s the Problem Here?

* `balance` is global
* Any function can change it
* No validation
* No security

This becomes dangerous in real-world systems like banking.

---

### Limitations of POP

* Poor security
* Code duplication
* No scalability
* Not suitable for large applications

POP works fine for small tasks but fails badly for large software.

---

## 4. Object Oriented Programming Paradigm

### What is a Programming Paradigm?

A **programming paradigm** is a style or philosophy of programming.

Examples:

* Procedural paradigm
* Object-oriented paradigm

---

### What is OOP Paradigm?

The **OOP paradigm** is based on:

* Objects
* Classes
* Data security
* Real-world modeling

It follows a **bottom-up approach**, meaning small objects are created first and then combined.

---

### Core Idea of OOP

> In OOP, **data is more important than functions**.

Instead of writing functions first, we design objects that represent real-world entities.

---

### OOP Example

```cpp
class BankAccount {
private:
    int balance;

public:
    void deposit() {
        balance += 100;
    }
};
```

Here:

* Data is hidden
* Only authorized functions can access it
* Security is maintained

---

## 5. Basic Concepts of Object Oriented Programming

---

### 5.1 Class

A **class** is a blueprint or template that defines:

* Data members (variables)
* Member functions (methods)

A class does not occupy memory until an object is created.

#### Example

```cpp
class Student {
    int roll;
    string name;
};
```

---

### 5.2 Object

An **object** is an instance of a class.
It represents a real-world entity and occupies memory.

```cpp
Student s1;
```

Here, `s1` is an object of class `Student`.

---

### 5.3 Encapsulation

Encapsulation means:

* Wrapping data and functions into one unit
* Restricting direct access to data

Encapsulation is achieved using:

* private
* protected
* public

---

#### Real-Life Example

ATM Machine:

* User interacts with buttons
* Internal logic is hidden
* Data is protected

---

#### C++ Example

```cpp
class Account {
private:
    int balance;

public:
    void setBalance(int b) {
        balance = b;
    }
};
```

Encapsulation improves **security and control**.

---

### 5.4 Abstraction

Abstraction means:

* Showing only essential details
* Hiding unnecessary implementation details

---

#### Real-Life Example

Driving a car:

* You use steering, accelerator, brake
* You don’t see engine details

---

Abstraction reduces complexity and improves usability.

---

### 5.5 Inheritance

Inheritance allows one class to:

* Reuse properties of another class
* Extend existing functionality

---

#### Example

```cpp
class Vehicle {
public:
    void start() {
        cout << "Vehicle started";
    }
};

class Car : public Vehicle {
};
```

Here:

* `Vehicle` is base class
* `Car` is derived class
* Code reuse is achieved

---

### 5.6 Polymorphism

Polymorphism means:

* One name, many forms
* Same function behaves differently

---

#### Example

```cpp
class Shape {
public:
    virtual void draw() {
        cout << "Drawing shape";
    }
};
```

Different shapes override `draw()` differently.

---

## 6. Benefits of Object Oriented Programming

### Why OOP is Better

1. **Data Security**

   * Data hiding using access specifiers

2. **Code Reusability**

   * Inheritance reduces duplication

3. **Easy Maintenance**

   * Changes are localized

4. **Real-World Representation**

   * Natural modeling of problems

5. **Scalability**

   * Easy to extend software

6. **Reduced Complexity**

   * Large problems divided into objects

---

## 7. Applications of Object Oriented Programming

OOP is used almost everywhere today.

### Major Applications

1. **Banking Systems**
2. **Railway Reservation Systems**
3. **Web Applications**
4. **Game Development**
5. **Mobile Applications**
6. **Enterprise Software**
7. **Simulation Systems**

---

## Conclusion

Procedure Oriented Programming is suitable for small programs, but modern software requires:

* Security
* Reusability
* Maintainability
* Scalability

**Object Oriented Programming using C++ provides all these features**, making it the backbone of modern software development.

---
