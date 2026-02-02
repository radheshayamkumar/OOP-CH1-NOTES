---

# Chapter 1: Object Oriented Programming using C++

---

## 1. Introduction to Object Oriented Programming (OOP)

Programming is the process of giving instructions to a computer to perform a specific task. In the early days, programs were small and simple, so traditional programming techniques worked fine. However, as software systems grew larger and more complex, these techniques became difficult to manage.

To solve these problems, **Object Oriented Programming (OOP)** was introduced.

**Object Oriented Programming (OOP)** is a programming approach in which software is designed using **objects** and **classes**, similar to real-world entities.

### Real-Life Example

Consider a **Car**:

* Attributes: color, speed, model
* Behaviors: start(), stop(), accelerate()

In OOP, we try to represent such real-world entities in software form. This makes programs easier to understand, design, and maintain.

C++ is an object-oriented language that supports the following OOP features:

* Classes
* Objects
* Encapsulation
* Abstraction
* Inheritance
* Polymorphism

---

## 2. Software Evolution

### Meaning of Software Evolution

Software evolution refers to the gradual development of programming techniques and languages to handle increasing software complexity and user requirements.

### Stages of Software Evolution

1. **Machine Language**

   * Uses binary digits (0s and 1s)
   * Very difficult to write, debug, and maintain
   * Machine dependent

2. **Assembly Language**

   * Uses mnemonics like MOV, ADD, SUB
   * Easier than machine language
   * Still machine dependent

3. **Procedure Oriented Programming (POP)**

   * Focus on procedures or functions
   * Example: C language
   * Suitable for small programs

4. **Object Oriented Programming (OOP)**

   * Focus on objects and data
   * Example: C++, Java, Python
   * Suitable for large and complex software systems

### Need for Software Evolution

* Increase in program size
* Poor data security
* Difficult maintenance
* Low code reusability

OOP evolved to overcome these limitations.

---

## 3. A Look at Procedure Oriented Programming (POP)

### What is Procedure Oriented Programming?

Procedure Oriented Programming is a programming approach in which:

* A program is divided into functions
* Functions operate on shared data
* Emphasis is on **logic and procedures**

### Characteristics of POP

* Top-down approach
* Functions are more important than data
* Global data access
* Less secure

### Example (POP Style)

```c
int balance;

void deposit() {
    balance += 100;
}

void withdraw() {
    balance -= 50;
}
```

In this example:

* `balance` is global
* Any function can modify it
* Data is not protected

### Limitations of POP

* Poor data security
* Difficult to manage large programs
* No real-world mapping
* Low code reusability

POP is suitable for small programs but not for large software systems.

---

## 4. Object Oriented Programming Paradigm

### Meaning of OOP Paradigm

A **programming paradigm** is a style or method of programming.

The **Object Oriented Programming paradigm** focuses on:

* Objects instead of functions
* Data security
* Real-world modeling
* Bottom-up approach

### Core Idea of OOP

> Data is more important than functions.

In OOP:

* Data and functions are combined together
* This combination is called a **class**

### Example

```cpp
class BankAccount {
    int balance;

public:
    void deposit() {
        balance += 100;
    }
};
```

Here, data is protected and accessed only through member functions.

---

## 5. Basic Concepts of Object Oriented Programming

### 5.1 Class

A **class** is a blueprint or template used to create objects. It defines the data members and member functions.

```cpp
class Student {
    int roll;
    string name;
};
```

---

### 5.2 Object

An **object** is an instance of a class. It represents a real-world entity.

```cpp
Student s1;
```

---

### 5.3 Encapsulation

Encapsulation means wrapping data and methods into a single unit and restricting direct access to data.

#### Real-Life Example

ATM Machine:

* User sees only buttons
* Internal logic is hidden

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

Encapsulation improves data security.

---

### 5.4 Abstraction

Abstraction means showing only essential details and hiding unnecessary information.

#### Example

Driving a car:

* You use accelerator, brake, and steering
* You don’t need to know engine internals

Abstraction reduces complexity.

---

### 5.5 Inheritance

Inheritance allows one class to acquire properties and behaviors of another class.

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

Here, `Car` inherits features of `Vehicle`.

---

### 5.6 Polymorphism

Polymorphism means **one name, multiple forms**.

```cpp
class Shape {
public:
    virtual void draw() {
        cout << "Drawing shape";
    }
};
```

The same function behaves differently based on the object.

---

## 6. Benefits of Object Oriented Programming

### Advantages of OOP

1. **Data Security**

   * Data hiding using access specifiers

2. **Code Reusability**

   * Achieved through inheritance

3. **Easy Maintenance**

   * Changes affect limited parts of code

4. **Real-World Modeling**

   * Programs resemble real-life objects

5. **Scalability**

   * Easy to expand and upgrade software

6. **Reduced Complexity**

   * Large problems divided into smaller objects

---

## 7. Applications of Object Oriented Programming

OOP is widely used in modern software development.

### Major Applications

1. **Real-Time Systems**

   * Banking systems
   * Railway reservation systems

2. **Web Applications**

   * E-commerce websites
   * Online portals

3. **Game Development**

   * Characters, weapons, and levels as objects

4. **Simulation Systems**

   * Traffic simulation
   * Weather forecasting

5. **Mobile Applications**

   * Android and iOS apps

6. **Enterprise Software**

   * ERP and CRM systems

---

## Conclusion

Procedure Oriented Programming is suitable for small applications, but modern software systems require:

* Security
* Reusability
* Maintainability
* Scalability

**Object Oriented Programming using C++ provides all these features**, making it an essential programming paradigm for today’s software development.

---
