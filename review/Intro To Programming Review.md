
# Table of Contents
1. [Introduction to C# Programming](#introduction-to-c-programming)
   - [What is C#?](#what-is-c)
   - [What is a Computer Program?](#what-is-a-computer-program)
   - [Hello, World! Program](#hello-world-program)
     - [Example](#example)
2. [Basic Syntax and Rules](#basic-syntax-and-rules)
   - [Syntax Basics](#syntax-basics)
3. [Understanding Input and Output in C#](#understanding-input-and-output-in-c)
   - [Basic Output in C#](#basic-output-in-c)
     - [Displaying Text](#displaying-text)
     - [String Concatenation](#string-concatenation)
     - [String Interpolation](#string-interpolation)
   - [Basic Input in C#](#basic-input-in-c)
     - [Reading from Console](#reading-from-console)
     - [Parsing User Input](#parsing-user-input)
4. [Understanding Arithmetic in C#](#understanding-arithmetic-in-c)
   - [Introduction to Arithmetic Operations](#introduction-to-arithmetic-operations)
   - [Basic Arithmetic Operators](#basic-arithmetic-operators)
     - [Addition (+)](#addition-)
     - [Subtraction (-)](#subtraction-)
     - [Multiplication (*)](#multiplication-)
     - [Division (/)](#division-)
     - [Modulus (%)](#modulus-)
   - [Using Arithmetic in Programs](#using-arithmetic-in-programs)
     - [Combining Operators](#combining-operators)
     - [Increment and Decrement Operators](#increment-and-decrement-operators)
   - [Advanced Arithmetic Concepts](#advanced-arithmetic-concepts)
     - [Working with Decimals](#working-with-decimals)
     - [Arithmetic with Mixed Data Types](#arithmetic-with-mixed-data-types)
     - [Complex Expressions and Order of Operations](#complex-expressions-and-order-of-operations)
5. [Understanding Conditionals and Boolean Logic in C#](#understanding-conditionals-and-boolean-logic-in-c)
   - [Introduction to Conditionals and Boolean Logic](#introduction-to-conditionals-and-boolean-logic)
   - [Basic Conditionals](#basic-conditionals)
     - [If Statement](#if-statement)
     - [If-Else Statement](#if-else-statement)
     - [Nested If](#nested-if)
   - [Boolean Logic](#boolean-logic)
     - [Boolean Operators](#boolean-operators)
     - [Comparison Operators](#comparison-operators)
   - [Advanced Conditional Structures](#advanced-conditional-structures)
     - [Switch Statement](#switch-statement)
     - [Conditional (Ternary) Operator](#conditional-ternary-operator)
6. [Understanding Data Types in C#](#understanding-data-types-in-c)
   - [Introduction to Data Types](#introduction-to-data-types)
   - [Primitive Data Types](#primitive-data-types)
     - [Integer Types](#integer-types)
     - [Floating Point Types](#floating-point-types)
     - [Char and Bool](#char-and-bool)
   - [Non-Primitive Data Types](#non-primitive-data-types)
     - [String Type](#string-type)
     - [Arrays](#arrays)
   - [Data Type Conversion](#data-type-conversion)
     - [Implicit Conversion](#implicit-conversion)
     - [Explicit Conversion](#explicit-conversion)
     - [Conversion Using Convert Class](#conversion-using-convert-class)
7. [Understanding Functions in C#](#understanding-functions-in-c)
   - [Introduction to Functions](#introduction-to-functions)
   - [Defining and Calling Functions](#defining-and-calling-functions)
     - [Basic Function Structure](#basic-function-structure)
     - [Calling a Function](#calling-a-function)
   - [Function Parameters and Return Types](#function-parameters-and-return-types)
     - [Parameters](#parameters)
     - [Return Types](#return-types)
8. [Understanding Repetition Structures in C#](#understanding-repetition-structures-in-c)
   - [Introduction to Repetition Structures](#introduction-to-repetition-structures)
   - [The For Loop](#the-for-loop)
     - [Basic For Loop](#basic-for-loop)
     - [Nested For Loops](#nested-for-loops)
   - [The While Loop](#the-while-loop)
     - [Basic While Loop](#basic-while-loop)
   - [The Do-While Loop](#the-do-while-loop)
     - [Basic Do-While Loop](#basic-do-while-loop)
   - [Break and Continue](#break-and-continue)
     - [Using Break](#using-break)
     - [Using Continue](#using-continue)

# Introduction to C# Programming

## What is C#?
C# (pronounced "C-Sharp") is a modern, object-oriented programming language developed by Microsoft. It is part of the .NET framework and is known for its simplicity and power. C# is widely used for developing desktop applications, web services, and mobile apps.

## What is a Computer Program?
A computer program is a set of instructions that a computer follows to perform a specific task. Programming involves writing these instructions in a programming language, like C#, that the computer can understand and execute.

## Hello, World! Program
The 'Hello, World!' program is a classic first program for beginners. It's a simple code that outputs "Hello, World!" to the console.

### Example
```csharp
using System;

namespace HelloWorld
{
    class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Hello, World!");
        }
    }
}
```

# Basic Syntax and Rules

## Syntax Basics
C# syntax is the set of rules that define the combinations of symbols that are considered to be correctly structured programs in the C# language.

### Comments
Comments are used to explain code or to make it more readable. They are completely ignored by the C# compiler.
- Single-line comment: `// This is a single-line comment`
- Multi-line comment: `/* This is a multi-line comment */`

### Semicolons
In C#, semicolons are used to denote the end of a statement.
- Example: `int number = 10;`

### Basic Syntax Rules
- C# is case-sensitive.
- Each line of instruction (statement) usually ends with a semicolon.
- The program execution starts from the `Main` method.

# Understanding Input and Output in C#
## Basic Output in C#

### Displaying Text
- The `Console.WriteLine()` method is used to display text on the console. It adds a new line at the end of the output.
- Example:
  ```csharp
  Console.WriteLine("Hello, World!");
  ```

### String Concatenation
- You can combine strings and variables to create more dynamic outputs.
- Example:
  ```csharp
  string name = "Alice";
  Console.WriteLine("Hello, " + name);
  ```

### String Interpolation
- A more modern approach to create strings with embedded expressions.
- Example:
  ```csharp
  int age = 30;
  Console.WriteLine($"Alice is {age} years old.");
  ```


## Basic Input in C#

### Reading from Console
- The `Console.ReadLine()` method is used for reading a line of text from the user input.
- Example:
  ```csharp
  Console.Write("Enter your name: ");
  string userName = Console.ReadLine();
  ```

### Parsing User Input
- Converting the string input to other data types like int, double, etc.
- Example:
  ```csharp
  Console.Write("Enter your age: ");
  int userAge = int.Parse(Console.ReadLine());
  ```

## Conclusion
These skills form the foundation of interacting with users in console applications. Practice these concepts to become proficient in handling data input and output in C#.

# Understanding Arithmetic in C#

## Introduction to Arithmetic Operations
Arithmetic in programming is used to perform mathematical operations between numbers. These operations are fundamental in processing and manipulating data.

## Basic Arithmetic Operators

### Addition (+)
- Used to add two numbers.
- Example:
  ```csharp
  int sum = 5 + 3; // sum is 8
  ```

### Subtraction (-)
- Used to subtract one number from another.
- Example:
  ```csharp
  int difference = 10 - 4; // difference is 6
  ```

### Multiplication (*)
- Used to multiply two numbers.
- Example:
  ```csharp
  int product = 6 * 7; // product is 42
  ```

### Division (/)
- Used to divide one number by another.
- Note: When dividing two integers, the result is an integer.
- Example:
  ```csharp
  int quotient = 20 / 4; // quotient is 5
  ```

### Modulus (%)
- Used to find the remainder of a division operation.
- Particularly useful in determining if a number is even or odd.
- Example:
  ```csharp
  int remainder = 7 % 3; // remainder is 1
  ```

## Using Arithmetic in Programs

### Combining Operators
- Operators can be combined to form complex expressions.
- Example:
  ```csharp
  int result = (5 + 3) * 2; // result is 16
  ```

### Increment and Decrement Operators
- `++` increments a value by 1.
- `--` decrements a value by 1.
- Example:
  ```csharp
  int counter = 10;
  counter++; // counter is now 11
  ```

## Advanced Arithmetic Concepts

### Working with Decimals
- Using `double` or `float` for decimal numbers.
- Example:
  ```csharp
  double divisionResult = 10.0 / 4.0; // divisionResult is 2.5
  ```

### Arithmetic with Mixed Data Types
- Mixing different data types in arithmetic operations.
- Data type conversion is often required.
- Example:
  ```csharp
  int integer = 5;
  double decimalNumber = 6.2;
  double mixResult = integer + decimalNumber; // mixResult is 11.2
  ```

### Complex Expressions and Order of Operations
- Understanding the precedence of operators.
- Using parentheses to control the order of operations.
- Example:
  ```csharp
  int complexResult = (2 + 3) * (5 - 2); // complexResult is 15
  ```

  # Understanding Conditionals and Boolean Logic in C#

## Introduction to Conditionals and Boolean Logic
Conditionals and Boolean logic are fundamental concepts in programming, enabling decision-making based on certain conditions. These concepts allow programs to execute different code blocks depending on the evaluation of boolean expressions.

## Conclusion
Arithmetic is a cornerstone of programming, allowing for the manipulation and calculation of numeric data. Mastery of these concepts is essential for effective programming in C#. Experiment with these operations and integrate them into your programs to enhance their functionality.


## Basic Conditionals

### If Statement
- The simplest form of conditional.
- Executes a block of code if a specified condition is true.
- Example:
  ```csharp
  if (temperature > 30) {
    Console.WriteLine("It's hot outside.");
  }
  ```

### If-Else Statement
- Extends the if statement to execute an alternative block of code if the condition is false.
- Example:
  ```csharp
  if (temperature > 30) {
    Console.WriteLine("It's hot outside.");
  } else {
    Console.WriteLine("It's not hot outside.");
  }
  ```

### Nested If
- If statements can be nested inside others to create more complex decision structures.
- Example:
  ```csharp
  if (temperature > 30) {
    if (isSunny) {
      Console.WriteLine("It's a hot and sunny day.");
    }
  }
  ```

## Boolean Logic

### Boolean Operators
- AND (`&&`), OR (`||`), NOT (`!`).
- Used to combine or invert boolean expressions.
- Example:
  ```csharp
  if (temperature > 30 && isSunny) {
    Console.WriteLine("It's a hot and sunny day.");
  }
  ```

### Comparison Operators
- `==`, `!=`, `<`, `>`, `<=`, `>=`.
- Used to compare values in boolean expressions.
- Example:
  ```csharp
  if (age >= 18) {
    Console.WriteLine("You are an adult.");
  }
  ```

## Advanced Conditional Structures

### Switch Statement
- An alternative to multiple if-else statements.
- More readable when checking a variable against multiple values.
- Example:
  ```csharp
  switch (grade) {
    case 'A':
      Console.WriteLine("Excellent!");
      break;
    case 'B':
      // ...
    default:
      Console.WriteLine("Grade not recognized.");
      break;
  }
  ```

### Conditional (Ternary) Operator
- A compact form of the if-else statement.
- Syntax: `condition ? expr1 : expr2`
- Example:
  ```csharp
  string result = age >= 18 ? "Adult" : "Minor";
  ```

## Conclusion
Conditionals and Boolean logic are critical for creating dynamic and responsive programs. They enable the program to make decisions and execute different code paths based on varying conditions. Understanding and effectively using these concepts is key to building functional and intelligent applications in C#.


# Understanding Data Types in C#

## Introduction to Data Types
Data types are an essential aspect of programming languages. They define the type of data a variable can hold, such as integers, floating-point numbers, characters, or strings.

## Primitive Data Types

### Integer Types
- `int`: Represents an integer.
- `long`: Larger range than `int`.
- Example:
  ```csharp
  int count = 10;
  long largeNumber = 5000000000;
  ```

### Floating Point Types
- `float`: Single-precision floating-point.
- `double`: Double-precision floating-point.
- Example:
  ```csharp
  float temperature = 25.3f;
  double pi = 3.14159;
  ```

### Char and Bool
- `char`: Represents a single character.
- `bool`: Represents a boolean (true/false).
- Example:
  ```csharp
  char grade = 'A';
  bool isPassed = true;
  ```

## Non-Primitive Data Types

### String Type
- `string`: Represents a sequence of characters.
- Example:
  ```csharp
  string name = "Alice";
  ```

### Arrays
- Holds a fixed number of values of a single type.
- Example:
  ```csharp
  int[] numbers = {1, 2, 3, 4, 5};
  ```

## Data Type Conversion

### Implicit Conversion
- Automatic conversion from a smaller to a larger data type.
- Example:
  ```csharp
  int num = 123;
  double bigNum = num;
  ```

### Explicit Conversion
- Also known as casting, used for converting a larger type to a smaller type.
- Example:
  ```csharp
  double pi = 3.14159;
  int intPi = (int)pi;
  ```

### Conversion Using Convert Class
- Using the `Convert` class for different conversions.
- Example:
  ```csharp
  string numberString = "123";
  int num = Convert.ToInt32(numberString);
  ```

## Conclusion
Understanding data types is crucial in programming as it affects how data is stored, manipulated, and interpreted. Each data type serves a specific purpose, and selecting the appropriate type for a variable is a fundamental skill in C# programming.


# Understanding Functions in C#

## Introduction to Functions
Functions in programming are used to encapsulate a set of instructions that perform a specific task. They improve code readability, reusability, and maintainability.

## Defining and Calling Functions

### Basic Function Structure
- Functions consist of a return type, name, parameters, and a body.
- Example:
  ```csharp
  void Greet(string name) {
    Console.WriteLine($"Hello, {name}!");
  }
  ```

### Calling a Function
- To execute a function, you call it by its name and pass any required arguments.
- Example:
  ```csharp
  Greet("Alice"); // Outputs: Hello, Alice!
  ```

## Function Parameters and Return Types

### Parameters
- Functions can take parameters, which are inputs used within the function.
- Example:
  ```csharp
  int Add(int a, int b) {
    return a + b;
  }
  ```

### Return Types
- The return type specifies the type of value the function will return.
- `void` is used when no value is returned.
- Example:
  ```csharp
  int Multiply(int x, int y) {
    return x * y;
  }
  ```

## Conclusion
Functions are a vital part of C# programming. They help to organize code into manageable sections and promote code reuse. Understanding how to define, call, and utilize functions effectively is key to becoming a proficient C# programmer.


# Understanding Repetition Structures in C#

## Introduction to Repetition Structures
Repetition structures, also known as loops, are used in programming to repeat a block of code multiple times. They are essential for tasks that require repetitive actions.

## The For Loop

### Basic For Loop
- Used for a known number of iterations.
- Consists of an initializer, condition, and incrementer.
- Example:
  ```csharp
  for (int i = 0; i < 5; i++) {
    Console.WriteLine($"Loop iteration: {i}");
  }
  ```

### Nested For Loops
- A for loop inside another for loop.
- Useful for working with multi-dimensional data structures.
- Example:
  ```csharp
  for (int i = 0; i < 3; i++) {
    for (int j = 0; j < 3; j++) {
      Console.WriteLine($"i = {i}, j = {j}");
    }
  }
  ```

## The While Loop

### Basic While Loop
- Repeats a block of code as long as a condition is true.
- The condition is evaluated before the loop body.
- Example:
  ```csharp
  int count = 0;
  while (count < 5) {
    Console.WriteLine($"Count: {count}");
    count++;
  }
  ```

## The Do-While Loop

### Basic Do-While Loop
- Similar to the while loop, but the condition is evaluated after the loop body.
- Ensures that the loop body is executed at least once.
- Example:
  ```csharp
  int number;
  do {
    number = int.Parse(Console.ReadLine());
  } while (number <= 0);
  ```

## Break and Continue

### Using Break
- Immediately exits the loop, regardless of the loop condition.
- Example:
  ```csharp
  for (int i = 0; i < 10; i++) {
    if (i == 5) break;
    Console.WriteLine(i);
  }
  ```

### Using Continue
- Skips the current iteration and proceeds to the next iteration.
- Example:
  ```csharp
  for (int i = 0; i < 10; i++) {
    if (i % 2 == 0) continue;
    Console.WriteLine(i);
  }
  ```

## Conclusion
Repetition structures are a fundamental concept in programming, allowing for the efficient execution of repetitive tasks. Understanding and effectively using these structures is crucial for creating dynamic and efficient C# programs.
