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
Boolean: 1
*/
```

## 4 control Structures
Control flow refers to the order in which statements are executed in a program. In C++, various control structures allow you to control the flow of execution based on conditions and loops.

### 1. If-Else Statements
The if-else statement allows you to execute different blocks of code based on conditions.

Syntax:
```cpp
if (condition) {
    // code block to execute if condition is true
} else {
    // code block to execute if condition is false
}
```
Example:
```cpp

#include <iostream>

int main() {
    int num = 10;

    if (num > 0) {
        std::cout << "Positive" << std::endl;
    } else {
        std::cout << "Non-positive" << std::endl;
    }

    return 0;
}
```

### 2. Switch Statement
The switch statement allows you to select one of many code blocks to be executed.

Syntax:
```cpp
switch (expression) {
    case value1:
        // code block
        break;
    case value2:
        // code block
        break;
    default:
        // default code block
}
```
Example:
```cpp
#include <iostream>

int main() {
    char grade = 'B';

    switch (grade) {
        case 'A':
            std::cout << "Excellent" << std::endl;
            break;
        case 'B':
            std::cout << "Good" << std::endl;
            break;
        default:
            std::cout << "Invalid grade" << std::endl;
    }

    return 0;
}
```

### 3. Loops

### a. For Loop
The for loop is used to execute a block of code a specified number of times.

Syntax:
```cpp

for (initialization; condition; increment/decrement) {
    // code block to execute
}
```
Example:
```cpp
#include <iostream>

int main() {
    for (int i = 0; i < 5; ++i) {
        std::cout << "Iteration " << i + 1 << std::endl;
    }

    return 0;
}
```
### b. While Loop
The while loop is used to execute a block of code as long as a specified condition is true.

Syntax:
```cpp
while (condition) {
    // code block to execute
}
```

Example:
```cpp
#include <iostream>

int main() {
    int i = 0;

    while (i < 5) {
        std::cout << "Iteration " << i + 1 << std::endl;
        ++i;
    }

    return 0;
}
```
### c. Do-While Loop
The do-while loop is similar to the while loop, but it executes the code block once before checking the condition.

Syntax:
```cpp
do {
    // code block to execute
} while (condition);
```

Example:
```cpp

#include <iostream>

int main() {
    int i = 0;

    do {
        std::cout << "Iteration " << i + 1 << std::endl;
        ++i;
    } while (i < 5);

    return 0;
}
```
### 4. Branching Statements
### a. Break Statement
The break statement is used to exit a loop or switch statement.

Example:
```cpp

#include <iostream>

int main() {
    for (int i = 0; i < 5; ++i) {
        if (i == 3) {
            break;
        }
        std::cout << "Iteration " << i + 1 << std::endl;
    }

    return 0;
}
```

### b. Continue Statement
The continue statement is used to skip the rest of the loop's code block and continue with the next iteration.

Example:
```cpp

#include <iostream>

int main() {
    for (int i = 0; i < 5; ++i) {
        if (i == 2) {
            continue;
        }
        std::cout << "Iteration " << i + 1 << std::endl;
    }

    return 0;
}
```

### c. Goto Statement
The goto statement is used to transfer control to another part of the program.

Example:
```cpp
#include <iostream>

int main() {
    int i = 0;

    loop:
    std::cout << "Iteration " << i + 1 << std::endl;
    ++i;
    if (i < 5) {
        goto loop;
    }

    return 0;
}
```


