# C++ Full Course

Welcome to the comprehensive C++ course! In this course, you will learn everything you need to know about the C++ programming language, from the basics to advanced topics. Each section includes detailed explanations, examples, and outputs to help you understand and practice C++ programming effectively.

## Table of Contents

1. [Introduction to C++](#1-introduction-to-c++)
2. [Basic Syntax](#2-basic-syntax)
3. [Data Types](#3-data-types)
4. [Control Structures](#4-control-structures)
5. [Functions](#5-functions)
6. [Arrays and Strings](#6-arrays-and-strings)
7. [Pointers](#7-pointers)
8. [Classes and Objects](#8-classes-and-objects)
9. [Inheritance](#9-inheritance)
10. [Polymorphism](#10-polymorphism)
11. [File Handling](#11-file-handling)
12. [Templates](#12-templates)
13. [Standard Template Library (STL)](#13-standard-template-library-stl)

---


##  1. Introduction to C++

C++ is a powerful and widely used programming language known for its efficiency and versatility. Developed by Bjarne Stroustrup as an extension of the C programming language, C++ supports both procedural and object-oriented programming paradigms and is used extensively in various domains such as systems programming, game development, and high-performance applications.

### Example:
```cpp
#include <iostream>

int main() {
    std::cout << "Hello, World!" << std::endl;
    return 0;
}
//Output
//Hello, World!
```
## 2. Basic Syntax

### Explanation:
The syntax of C++ includes various elements such as keywords, identifiers, operators, etc. Understanding the basic syntax is essential for writing C++ programs.

Example:
```cpp
#include <iostream>

int main() {
    // This is a single-line comment

    /*
     * This is a
     * multi-line comment
     */

    int num1 = 10;
    int num2 = 20;
    int sum = num1 + num2;

    std::cout << "Sum: " << sum << std::endl;

    return 0;
}

//Output:
//Sum: 30
```

## 3. Data Types

Data types in C++ specify the type of data that a variable can hold. C++ supports various data types such as:

### Primitive Data Types: Integers, Floating-point numbers, Characters, Booleans
### Derived Data Types: Arrays, Pointers, References
### User-defined Data Types: Structures, Classes, Enums

Understanding data types is crucial for defining variables and manipulating data effectively.

Example:
```cpp
#include <iostream>

int main() {
    int num = 10;
    float floatValue = 3.14;
    char charValue = 'A';
    bool boolValue = true;

    std::cout << "Integer: " << num << std::endl;
    std::cout << "Float: " << floatValue << std::endl;
    std::cout << "Character: " << charValue << std::endl;
    std::cout << "Boolean: " << boolValue << std::endl;

    return 0;
}
/*
Output:
Integer: 10
Float: 3.14
Character: A
*/Boolean: 1

