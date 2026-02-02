---

````md
# Chapter 1: Object Oriented Programming using C++

---

## 1. Introduction to Object Oriented Programming (OOP)

Programming is the process of giving instructions to a computer to solve a problem. As software systems became larger and more complex, traditional programming approaches started failing due to poor structure, low security, and difficult maintenance.

To overcome these problems, **Object Oriented Programming (OOP)** was introduced.

**Object Oriented Programming (OOP)** is a programming approach where a program is designed using **objects** and **classes**, similar to real-world entities.

### Real-Life Example:
- **Car** → Object  
- **Attributes** → Color, speed, model  
- **Behaviors** → start(), stop(), accelerate()

OOP tries to model software in the same way we observe the real world, making programs easier to design, understand, and maintain.

C++ supports major OOP concepts such as:
- Classes
- Objects
- Encapsulation
- Inheritance
- Polymorphism
- Abstraction

---

## 2. Software Evolution

### What is Software Evolution?
Software evolution refers to the gradual development of programming techniques to handle increasing software complexity.

### Stages of Software Evolution:

1. **Machine Language**
   - Uses binary digits (0s and 1s)
   - Very difficult to write and debug

2. **Assembly Language**
   - Uses mnemonics like MOV, ADD
   - Still machine dependent

3. **Procedure Oriented Programming (POP)**
   - Focus on functions
   - Example: C language

4. **Object Oriented Programming (OOP)**
   - Focus on objects and data
   - Example: C++, Java, Python

### Why Evolution Was Necessary?
- Increasing software size
- Poor code reusability
- Difficult debugging
- Lack of data security

OOP addressed these issues by organizing software around **objects instead of functions**.

---

## 3. A Look at Procedure Oriented Programming (POP)

### What is POP?
Procedure Oriented Programming is a programming approach where:
- A program is divided into functions
- Data is shared among functions
- Functions control program flow

### Key Characteristics of POP:
- Emphasis on functions
- Global data access
- Top-down programming approach
- Difficult to manage large programs

### Example (POP Style Code):
```c
int balance;

void deposit() {
    balance += 100;
}

void withdraw() {
    balance -= 50;
}
````

Here, data (`balance`) is global and unprotected, which can cause serious issues.

### Limitations of POP:

* Poor data security
* No real-world representation
* Low code reusability
* Difficult maintenance

POP is suitable for small programs but fails for large-scale software.

---

## 4. Object Oriented Programming Paradigm

### What is an OOP Paradigm?

A **programming paradigm** is a style or method of programming.

The **OOP paradigm** focuses on:

* Objects
* Data security
* Real-world modeling
* Bottom-up approach

### Core Idea:

> Data is more important than functions.

In OOP:

* Data and functions are combined into a single unit
* This unit is called a **class**

### Example:

```cpp
class BankAccount {
    int balance;

public:
    void deposit() {
        balance += 100;
    }
};
```

Data is protected and accessed only through defined methods.

---

## 5. Basic Concepts of Object Oriented Programming

### 5.1 Class

A **class** is a blueprint or template used to create objects.

```cpp
class Student {
    int roll;
    string name;
};
```

---

### 5.2 Object

An **object** is an instance of a class.

```cpp
Student s1;
```

---

### 5.3 Encapsulation

Encapsulation means wrapping data and methods into a single unit and restricting direct access to data.

#### Real-Life Example:

ATM Machine

* User accesses only buttons
* Internal processing is hidden

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

---

### 5.4 Abstraction

Abstraction means showing only essential features and hiding unnecessary details.

#### Example:

Driving a car

* Controls are visible
* Engine mechanism is hidden

---

### 5.5 Inheritance

Inheritance allows one class to acquire properties of another class.

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

---

### 5.6 Polymorphism

Polymorphism means **one interface, multiple implementations**.

```cpp
class Shape {
public:
    virtual void draw() {
        cout << "Drawing shape";
    }
};
```

---

## 6. Benefits of Object Oriented Programming

### Advantages of OOP:

1. **Improved Data Security**

   * Data hiding using access specifiers

2. **Code Reusability**

   * Achieved using inheritance

3. **Easy Maintenance**

   * Changes affect limited parts of code

4. **Real-World Modeling**

   * Programs mirror real-life objects

5. **Scalability**

   * Easy to extend applications

6. **Reduced Complexity**

   * Large problems divided into objects

---

## 7. Applications of Object Oriented Programming

OOP is widely used in modern software development.

### Applications Include:

1. **Real-Time Systems**

   * Banking systems
   * Railway reservation systems

2. **Web Applications**

   * E-commerce platforms
   * Online portals

3. **Game Development**

   * Characters, weapons, levels as objects

4. **Simulation Systems**

   * Traffic systems
   * Weather forecasting

5. **Mobile Applications**

   * Android and iOS apps

6. **Enterprise Software**

   * ERP and CRM systems

---

## Conclusion

Procedure Oriented Programming is suitable for small programs, but modern software requires:

* Security
* Reusability
* Maintainability
* Scalability

**Object Oriented Programming using C++ fulfills these requirements**, making it a powerful and essential programming paradigm.

---

```

---

