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


## 1. Introduction to C++

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
## 5. Functions

Functions in C++ are blocks of code that perform a specific task. They are essential for organizing code, promoting reusability, and improving readability.

## Explanation

A function in C++ consists of a function header and a function body. The header contains the function's signature, including the return type, function name, and parameters. The body contains the code that defines the function's behavior.

### Syntax

```cpp
return_type function_name(parameter_list) {
    // function body
}
```

### return_type: 
The data type of the value returned by the function. It can be void if the function does not return any value.

### function_name: 
The name of the function, which should be unique within its scope.

### parameter_list: 
The list of parameters passed to the function. Parameters are optional.

Example
```cpp
#include <iostream>

// Function declaration
int add(int a, int b) {
    return a + b;
}

int main() {
    int result = add(5, 3);
    std::cout << "Result: " << result << std::endl;
    return 0;
}
```


### Additional Notes
Functions can be defined either before or after the main() function. However, if a function is defined after main(), it must be declared before it.

A function can have default parameter values, allowing some parameters to be omitted during function calls.

Recursive functions are functions that call themselves. They are useful for solving problems that can be broken down into smaller, similar subproblems.

Functions play a crucial role in C++ programming, offering modularity and flexibility. Understanding how to define, declare, and use functions is essential for writing efficient and maintainable code.

## 6. Arrays and Strings

Arrays and strings are fundamental data structures in C++. Understanding how to work with arrays and strings is essential for developing a wide range of applications.

### Arrays

An array is a collection of elements of the same data type stored in contiguous memory locations. It allows you to store multiple values under a single name and access them using an index.

Example:
```cpp
#include <iostream>

int main() {
    int arr[5] = {1, 2, 3, 4, 5};

    // Accessing elements of the array
    for (int i = 0; i < 5; ++i) {
        std::cout << "Element " << i << ": " << arr[i] << std::endl;
    }

    return 0;
}
```
### Strings
A string in C++ is a sequence of characters stored in contiguous memory locations. It is represented using the std::string class from the Standard Template Library (STL).

Example:

```cpp
#include <iostream>
#include <string>

int main() {
    std::string str = "Hello, World!";

    // Accessing characters of the string
    for (char c : str) {
        std::cout << c;
    }

    return 0;
}
```
### 7. Pointers
Pointers are variables that store memory addresses. They allow you to indirectly access memory locations and manipulate data efficiently.

Example:
```cpp
#include <iostream>

int main() {
    int num = 10;
    int* ptr = &num;

    std::cout << "Value of num: " << num << std::endl;
    std::cout << "Address of num: " << &num << std::endl;
    std::cout << "Value of ptr: " << ptr << std::endl;
    std::cout << "Value pointed by ptr: " << *ptr << std::endl;

    return 0;
}
```

### 8. Classes and Objects
Classes and objects are fundamental concepts in object-oriented programming (OOP). They allow you to model real-world entities and encapsulate data and behavior within a single unit.

Example:
```cpp
#include <iostream>
#include <string>

class Student {
private:
    std::string name;
    int age;

public:
    // Constructor
    Student(std::string n, int a) {
        name = n;
        age = a;
    }

    // Member function
    void display() {
        std::cout << "Name: " << name << std::endl;
        std::cout << "Age: " << age << std::endl;
    }
};

int main() {
    // Creating an object of the Student class
    Student s("John", 20);

    // Accessing member function
    s.display();

    return 0;
}
```

### 9. Inheritance
Inheritance is a mechanism in C++ that allows a class to inherit properties and behavior from another class. It promotes code reusability and supports the concept of hierarchical relationships.

Example:
```cpp
#include <iostream>
#include <string>

// Base class
class Person {
protected:
    std::string name;
    int age;

public:
    Person(std::string n, int a) : name(n), age(a) {}

    void display() {
        std::cout << "Name: " << name << std::endl;
        std::cout << "Age: " << age << std::endl;
    }
};

// Derived class
class Student : public Person {
private:
    int rollNumber;

public:
    Student(std::string n, int a, int r) : Person(n, a), rollNumber(r) {}

    void displayRollNumber() {
        std::cout << "Roll Number: " << rollNumber << std::endl;
    }
};

int main() {
    // Creating an object of the Student class
    Student s("John", 20, 101);

    // Accessing member functions
    s.display();
    s.displayRollNumber();

    return 0;
}
```

### 10. Polymorphism
Polymorphism is a key concept in OOP that allows objects of different classes to be treated as objects of a common superclass. It enables dynamic binding and method overriding.

Example:

```cpp
#include <iostream>
#include <string>

// Base class
class Shape {
public:
    virtual void draw() {
        std::cout << "Drawing a shape" << std::endl;
    }
};

// Derived class
class Circle : public Shape {
public:
    void draw() override {
        std::cout << "Drawing a circle" << std::endl;
    }
};

int main() {
    // Creating objects of different classes
    Shape* s1 = new Shape();
    Shape* s2 = new Circle();

    // Calling the draw method
    s1->draw();
    s2->draw();

    return 0;
}
```

### 11. File Handling
File handling in C++ allows you to perform various operations such as reading from and writing to files. It provides classes and functions for working with files efficiently.

Example:
```cpp
#include <iostream>
#include <fstream>
#include <string>

int main() {
    std::ofstream file("example.txt");

    if (file.is_open()) {
        file << "Hello, World!";
        file.close();
        std::cout << "File written successfully." << std::endl;
    } else {
        std::cerr << "Unable to open file." << std::endl;
    }

    return 0;
}
```
### 12. Templates
Templates in C++ allow you to create generic functions and classes that can work with any data type. They promote code reuse and support type-safe programming.

Example:
```cpp
#include <iostream>

// Template function
template<typename T>
T add(T a, T b) {
    return a + b;
}

int main() {
    // Calling the template function with different data types
    std::cout << "Sum of integers: " << add(5, 3) << std::endl;
    std::cout << "Sum of floats: " << add(3.5, 2.7) << std::endl;

    return 0;
}
```

### 13. Standard Template Library (STL)
The Standard Template Library (STL) is a powerful library in C++ that provides various data structures and algorithms. It includes containers such as vectors, lists, maps, and algorithms such as sorting and searching.

Example:

```cpp
#include <iostream>
#include <vector>
#include <algorithm>

int main() {
    std::vector<int> numbers = {5, 2, 8, 1, 6};

    // Sorting the vector
    std::sort(numbers.begin(), numbers.end());

    // Displaying the sorted vector
    for (int num : numbers) {
        std::cout << num << " ";
    }
    std::cout << std::endl;

    return 0;
}
```
### 11. File Handling
File handling in C++ allows you to perform various operations such as reading from and writing to files. It provides classes and functions for working with files efficiently.

Example:

```cpp
#include <iostream>
#include <fstream>
#include <string>

int main() {
    std::ofstream file("example.txt");

    if (file.is_open()) {
        file << "Hello, World!";
        file.close();
        std::cout << "File written successfully." << std::endl;
    } else {
        std::cerr << "Unable to open file." << std::endl;
    }

    return 0;
}
```
### 12. Templates
Templates in C++ allow you to create generic functions and classes that can work with any data type. They promote code reuse and support type-safe programming.

Example:
```cpp
#include <iostream>

// Template function
template<typename T>
T add(T a, T b) {
    return a + b;
}

int main() {
    // Calling the template function with different data types
    std::cout << "Sum of integers: " << add(5, 3) << std::endl;
    std::cout << "Sum of floats: " << add(3.5, 2.7) << std::endl;

    return 0;
}
```

### 13. Standard Template Library (STL)
The Standard Template Library (STL) is a powerful library in C++ that provides various data structures and algorithms. It includes containers such as vectors, lists, maps, and algorithms such as sorting and searching.

Example:
```cpp
#include <iostream>
#include <vector>
#include <algorithm>

int main() {
    std::vector<int> numbers = {5, 2, 8, 1, 6};

    // Sorting the vector
    std::sort(numbers.begin(), numbers.end());

    // Displaying the sorted vector
    for (int num : numbers) {
        std::cout << num << " ";
    }
    std::cout << std::endl;

    return 0;
}
```
