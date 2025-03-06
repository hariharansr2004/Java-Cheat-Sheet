# Java

Java is a **Class-based, High-level, Object-Oriented Programming Language**.

## Key Features:
- **Platform Independent or Portable**
- **Object Oriented Language**
- **Security**
- **Rich API's**

## History:
- Developed by **Sun Microsystems** on **May 23, 1995**
- Developed by **James Gosling**
- Initial Names: **Oak, Green Talk**
- Later acquired by **Oracle Corporation**
- **JDK 1.0.2** was released on **Jan 23, 1996**
- **Open Distributed System Compiler** was released on **May 8, 2007**

## Applications:
Java is widely used in:
- Big Enterprise Applications
- Mobile Applications
- Desktop Applications
- Games
- Cloud Computing
- Big Data
- Artificial Intelligence

## Features of Java:
![z](https://github.com/user-attachments/assets/d36093cc-7e45-44a2-8bbe-6f728c2b2bc0)

<br>

## Platform Independence:
Java is a platform-independent language because:
- In any programming language, source code is compiled into executable code, which cannot run across all platforms.
- When Java compiles a program, it generates an executable file called a **.class** file. This class file contains **byte codes**.
- **Byte-code** is a special format of machine-level code [intermediate language] that is not tied to any operating system.
- Byte codes are interpreted only by the **JVM**. JVM is OS-dependent since it differs for different OS.
- Since these JVMs are made available across all platforms by **Sun Microsystems**, we can execute this byte code on any platform.
- A byte code generated in a **Windows** environment can also be executed in a **Linux** environment. This makes Java platform-independent.
- That’s why Java is called **WORA**.
- **WORA → Write Once, Run Anywhere**

[Watch this video](https://youtu.be/7yr81Dnn0NY?si=a5Yc6NEeBfCkoqlT) for more details.

![zp](https://github.com/user-attachments/assets/f30c99df-1027-47b1-8beb-2f93aa558c51)

<br>

## Java Architecture:

![image](https://github.com/user-attachments/assets/3a28630b-7162-4102-846f-110b0507cee6)

<br>

# Java Environment Components  

## 1. JDK (Java Development Kit)  
Java Development Kit provides the environment to develop and execute Java programs. It includes:  
- A **compiler**, an **archiver**, a **debugger**, and other development tools.  
- **Java Runtime Environment (JRE)** for executing Java programs.  

**Note:** JDK is platform-dependent, so separate installers are needed for Windows, Unix, and Mac operating systems.  

JDK mainly includes two components:  
- **Development Tools** – Provides an environment to develop Java programs.  
- **JRE** – Used to execute Java programs.  

<br>

## 2. JRE (Java Runtime Environment)  
Java Runtime Environment is a software package that provides an environment to **run** Java programs (not develop them).  

It contains:  
- **JVM (Java Virtual Machine)**  
- **Libraries and Other Components** required to run Java applications.  

**Note:** JRE is primarily for running Java applications, not for development.  

<br>

## 3. JVM (Java Virtual Machine)  
JVM is a virtual CPU that provides a runtime environment for executing Java bytecodes.  

It performs the following tasks:  
- Converts **bytecode** into **machine-specific code**.  
- Loads class files in the **class loader**.  
- Verifies bytecode with the **bytecode verifier**.  
- Executes bytecode line by line (hence, it acts as an **interpreter**).  

<br>

## 4. JIT (Just-In-Time Compiler)  
Just-In-Time Compiler is a part of the **JVM** that enhances the performance of Java applications by **compiling bytecodes to native machine code at runtime**.  

<br>

## ClassLoader

- Find and Loads Java Classes!

Three Types
- System Class Loader - Loads all application classes from CLASSPATH
- Extension Class Loader - Loads all classes from extension directory
- Bootstrap Class Loader - Loads all the Java core files

Order of execution of ClassLoaders
- JVM needs to find a class, it starts with System Class Loader. 
- If it is not found, it checks with Extension Class Loader. 
- If it not found, it goes to the Bootstrap Class Loader. 
- If a class is still not found, a ClassNotFoundException is thrown.

<br>

### Architecture of JDK, JRE, JVM:
![image](https://github.com/user-attachments/assets/cdf79a6f-aa70-4cd1-a516-4d1e8ab2e4a2)
<br>

### First Java Program

```java
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello World");
    }

}
```
## Compiling and Running Java Code
- Compile: javac HelloWorld.java
- Run: java HelloWorld
<br>

## What Happens if We Save a Blank File as a .java File?
- If you save a blank file with a `.java` extension and try to compile it using `javac`, the compiler will return an error.
- A `.java` file must contain at least one class or interface declaration. A blank file will not be considered a valid Java program by the compiler.
<br>

## Can We Perform Changes in Bytecode? What Are the Issues?
Yes, you can make changes to bytecode manually, but it’s highly discouraged due to several issues.

<br>


## Difference between C++ and Java

| Specifications        | C++                                              | Java                                                   |
|----------------------|--------------------------------------------------|--------------------------------------------------------|
| **Memory Management** | Use of Pointers & Structures                     | No user thread, user interface, object, Automatic Garbage Collection by default |
| **Libraries**         | Available with low-level Functionalities        | High level Services and wide range of classes         |
| **Multiple Inheritance** | Provides Multiple Inheritance                   | Multiple Inheritance is partially done by interface  |
| **Operator Overloading** | Supports Operator Overloading                   | Doesn’t Support Operator Overloading                  |
| **Portability**       | Platform Dependent                              | Platform Independent                                  |
| **Program Handling**  | Functions & variables reside outside the class | Functions & variables reside only in classes & packages |
| **Thread Support**    | No build & support in Thread Support. It depends only on the libraries | It has Built-in Thread Support |

<br>

## Datatypes in Java

Data types in Java are divided into two groups:

- **Primitive Data Types**:
 These data types are predefined by Java and named by a keyword. They are used to store simple values directly. It includes `byte`, `short`, `int`, `long`, `float`, `double`, `boolean`, and `char`.
- **Non-Primitive Data Types**:
  These data types are **not predefined**. They are also known as **reference variables** or **object references** in Java. It includes `String`, `Arrays`, `Classes`, `Objects`, and `Interfaces`.

## Memory Representation

- **1 Byte = 8 Bits**

![image](https://github.com/user-attachments/assets/3e1f316d-3c76-46e6-8320-cf0988bac31b)

## ASCII:
- ASCII- American Standard Code for Information Interchange
- Created in 1960 for encoding characters in computers and digital systems.
- Decimal Value for (a-z) : 65-90
- Decimal Value for (A-Z) : 97-122
<br>

# Size of Data Type in Java

This program demonstrates the size limitations of different data types in Java.

## Java Code:

```java
package com.datatypes;

/* Size of Data Type */

public class Jtc {
    public void dataType2() {
        System.out.println("---dataType2() in Jtc class---");
        byte b11 = 127;
        byte b22 = -128;
        // byte b33 = 128; // Error: 128 is out of range for byte
        // byte b44 = -129; // Error: -129 is out of range for byte
        int i11 = 2147483647;
        int i12 = -2147483648;
        // int i13 = 2147483648; // Error: 2147483648 is out of range for int
        // long l14 = 2147483649; // Error: 2147483649 is interpreted as int by default
        long l12 = 2147483648L; // Correct usage for long type
        // float f11 = 11.11; // Error: 11.11 is interpreted as double by default
        float f12 = 11.11f; // Correct usage for float type
        double d11 = 11.12;
        double d12 = 11.13d;
        
        System.out.println(b11);
        System.out.println(b22);
        System.out.println(i11);
        System.out.println(i12);
        System.out.println(l12);
        System.out.println(f12);
        System.out.println(d12);
    }

    public static void main(String[] args) {
        Jtc jtc = new Jtc();
        jtc.dataType2();
    }
}
```

## Explanation of Errors in Commented Code:

### 1. `byte b33 = 128;`
- **Error**: `128` is outside the range of the `byte` data type, which can only hold values from `-128` to `127`.

### 2. `byte b44 = -129;`
- **Error**: `-129` is also outside the range of the `byte` data type.

### 3. `int i13 = 2147483648;`
- **Error**: `2147483648` is out of range for the `int` type, which supports values from `-2147483648` to `2147483647`.

### 4. `long l14 = 2147483649;`
- **Error**: Although `2147483649` fits within the `long` range, it is treated as an `int` by default in Java. Adding an `L` at the end like `2147483648L` tells the compiler to treat it as a `long`.

### 5. `float f11 = 11.11;`
- **Error**: By default, decimal numbers in Java are treated as `double`. To store a value as a `float`, you must append `f` or `F` at the end, like `11.11f`.

<br>

## Range of Primitive Data Types
The range of a data type defines the maximum and minimum values that the type can hold.

## Java Code:
```java

/* Data Type Minimum and Maximum value */

public class Jtc {
    public void dataType3() {
        System.out.println("Byte Range: " + Byte.MIN_VALUE + " to " + Byte.MAX_VALUE);
        System.out.println("Short Range: " + Short.MIN_VALUE + " to " + Short.MAX_VALUE);
        System.out.println("int Range: " + Integer.MIN_VALUE + " to " + Integer.MAX_VALUE);
        System.out.println("Long Range: " + Long.MIN_VALUE + " to " + Long.MAX_VALUE);
        System.out.println("Float Range: " + Float.MIN_VALUE + " to " + Float.MAX_VALUE);
        System.out.println("Double Range: " + Double.MIN_VALUE + " to " + Double.MAX_VALUE);
    }

    public static void main(String[] args) {
        Jtc jtc = new Jtc();
        jtc.dataType3();
    }
}
```

## `print` and `println`

- `print()`: Outputs text on the same line.
- `println()`: Outputs text and then moves to the next line.

## Commenting Code in Java

Comments are notes ignored by the compiler, useful for explaining code.

### Single-line comment:
```java
// This is a single-line comment
```

### Multi-line comment:
```java
/*
This is a
multi-line comment
*/
```

### Documentation comment (used in JavaDoc):
```java
/**
 * This is a documentation comment
 * which can be used for JavaDoc.
 */
```

## Interview Questions Related to Java Basics

### 1. Is Java is pure Object Oriented Language?
- No, it’s partially object oriented because,it supports primitive data types like "int", "float", and "double", which are not objects.

### 2. Can we change the syntax of the main method?
No, JVM recognizes `public static void main(String[] args)` as the entry point, so it must remain unchanged for Java applications to run.

### 3. Can we keep the main method as private?
No, because JVM needs to access the `main` method from outside the class. If it’s private, the program will compile but not execute, resulting in an error.

### 4. Can we keep the main method non-static?
No, `main` is static so JVM can call it without creating an object. If it’s non-static, JVM cannot call it directly, and the program will not execute.

### 5. Why do we need `f` for float literals?
By default, decimal numbers are considered `double`. Adding `f` tells Java to treat the number as a `float`.

<br>

## Identifiers
Names given to a class, method, interface, variables are called identifiers.

Legal Identifier Names
- Combination of letters, numbers, $ and under-score(_)
- Cannot start with a number
- Cannot be a keyword
- No limit on length of identifier

## Java Keywords
List of Java Keywords
- Primitives DataTypes    : byte,short,int,long,float,double,char,boolean
- Flow Control    : if, else,for,do, while, switch, case, default, break,
      continue,return
- Exception Handling      : try, catch, finally,throw,throws,assert
- Modifiers       : public,private,protected,final,static,native,abstract,
      synchronized,transient,volatile,strictfp
- Class Related   : class,interface,package,extends,implements,import
- Object Related  : new, instanceof,super,this
- Literals    : true, false, null
- Others      : void, enum
- Unused  : goto,const

## Literals
Any primitive data type value in source code is called Literal.

There are four types of literals:
- Integer & Long
- Floating Point
- Boolean
- Double

#### Literals Types

Integer Literals
- There are 3 ways of representing an Integer Literal. 
  - Decimal. Examples: 343, 545
  - Octal. Digits 0 to 7. Place 0 before a number. Examples : 070,011
  - Hexadecimal. Digits 0 to 9 and alphabets A to F (10-15). Case insensitive.
- An integer literal by default is int.

Long Literals 
- All 3 integer formats: Decimal, Octal and Hexadecimal can be used to represent long by appending with L or l.

Floating point Literals
- Numbers with decimal points. Example: ```double d = 123.456;```
- To declare a float, append f. Example: float f = 123.456f;
- Floating point literals are double by default.
- Appending d or D at end of double literal is optional Example: ```double d = 123.456D;```

 Boolean Literals
- Valid boolean values are true and false. 
- TRUE, FALSE or True, False are invalid.

 Character Literals
- Represented by single character between single quotes  Example: ```char a = 'a'```
- Unicode Representation also can be used. Prefix with \u. Example: char letterA = '\u0041';
- A number value can also be assigned to character. Example: char letterB = 66; Numeric value can be from 0 to 65535;
- Escape code can be used to represent a character that cannot be typed as literal. Example: char newLine = '\n';

#### Puzzles 

```java
int eight = 010; 
int nine=011;  
int invalid = 089;//COMPILER ERROR! 8 and 9 are invalid in Octal
int sixteen = 0x10; 
int fifteen = 0XF; 
int fourteen = 0xe;
int x = 23,000;
long a = 123456789l; 
long b = 0x9ABCDEFGHL; 
long c = 0123456789L;

float f = 123.456;//COMPILER ERROR! A double value cannot be assigned to a float.

boolean b = true; boolean b=false;
boolean b = TRUE;//COMPILATION ERROR
boolean b = 0; //COMPILER ERROR. This is not C Language

char ch = a;
char a = 97;
char ch1 = 66000; //COMPILER ERROR!
```
<br>

## Java Operators

1. **Arithmetic Operators**: Perform basic arithmetic operations. (`+`, `-`, `*`, `/`, `%`).
2. **Unary Operators**: Operate on a single operand. (`++`, `--`).
   >  ++ Increments by 1.
   > > Post-Increment: Uses value first, then increments. Returns original value before incrementation.
   > > 
   > > Pre-Increment: Increments first, then uses value.
   > > 
   > -- Decrements by 1.
   > > Post-Decrement: Uses value first, then decrements. Returns original value before decrementation.
   > > 
   > > Pre-Decrement: Decrements first, then uses value.

4. **Assignment Operators**: Assign values with operations. (`+=`, `-=`, `*=`, `/=`, `%=`).
5. **Relational Operators**: Compare values, returning boolean. (`==`, `!=`, `>`, `<`, `>=`, `<=`).
6. **Logical Operators**: Perform logical operations.They have a short-circuiting effect, meaning the second condition is not evaluated if the first is false (`&&`, `||`, `!`).
7. **Ternary Operator**: Shortened if-else statement. (`condition ? if true : if false`).
8. **Bitwise Operators**: Operate at the bit level. (`&`, `|`, `^`, `~`).
9. **Shift Operators**: Shift bits left or right. (`<<`, `>>`, `>>>`).
10. **`instanceof` Operator**: Checks object type. (`obj instanceof Class`).
    
![image](https://github.com/user-attachments/assets/9fe7b8f9-83a5-498f-97b0-56e094b69f87)

<br>

# Variables in Java


## 1. Instance Variables

An **instance variable** is a variable that belongs to an object (instance) of a class. It is declared inside a class but outside any method. 

### Characteristics:
- Created when an object of the class is instantiated.
- Each object of the class has its own copy.
- Stores unique data for each instance.
- Cannot be accessed in a static context directly.

### Example:
```java
class Student {
    int sid;  // Instance variable for student ID
    String sname;  // Instance variable for student name
    String semail;  // Instance variable for student email
}
```
<br>

## 2. Static Variables

A **static variable** is a class-level variable shared among all instances of the class. It is declared using the `static` keyword.

### Characteristics:
- Belongs to the class rather than any individual object.
- Memory is allocated only once when the class is loaded.
- Can be accessed using the class name.
- Shared across all instances of the class.
  
### Example:
```java
class A {
    static int a = 10; // Static variable
}

class Main {
    public static void main(String[] args) {
        System.out.println(A.a);  // Access using class name
        A obj = new A();
        System.out.println(obj.a);  // Access using object
    }
}
```
<br>

## 3. Local Variables

- Local variables are declared within a method, constructor, or block.
- They must be initialized before use, as they do not have default values.

### Is Initialization of Local Variables Mandatory?
**Yes**, it is mandatory to initialize local variables. If we do not initialize them, we will get a compile-time error saying:
```
Variable might not be initialized
```

### Characteristics:
- Memory for local variables is allocated only when the method or block is executed and is released when it ends.
- Local variables can only be `default` or `final`, i.e., we cannot declare a local variable as `private`, `public`, or `protected`.

### Key Differences Between Class Level and Local Variables:
![image](https://github.com/user-attachments/assets/cee6d31f-8b23-41f1-86a5-475ca3e900b0)


## Diff b/w instance ans static variable
| Feature | Instance Variable | Static Variable |
|---------|------------------|----------------|
| Declaration | Inside class, outside methods | Inside class, outside methods with `static` keyword |
| Memory Allocation | Created when an object is instantiated | Created when the class is loaded |
| Access | Through an object | Through class name or object |
| Data Sharing | Unique per object | Shared among all objects |
| Can be used in static methods? | ❌ No | ✅ Yes |


### Q. What if local variable and global variable names are same?
- If local var and global var names are same first priority is always given to local variables because they are inside method and nearer for execution to JVM.
<br>

### Scope of a Variable
- Scope of a variable defines where (which part of code) a variable can be accessed.

#### Important Rules
- Static Variable can be used anywhere in the class.
- Member Variable can be used in any non-static method.
- Local Variable can be used only in the method where it is declared.
- Block Variable can be used only in the block (code between { and }) where it is declared.
  
#### Variable Scope Examples
Below code shows all these Rules in action:
```java

public class VariablesExample {
    //RULE 1:Static Variable can be used anywhere in the class. 
    static int staticVariable;
    
    //RULE 2:Member Variable can be used in any non-static method. 
    int memberVariable;
    
    void method1() {
		//RULE 3: method1LocalVariable can be used only in method1.
		int method1LocalVariable;

		memberVariable = 5;//RULE 2
		staticVariable = 5;//RULE 1

		//Some Code
		{
		    //RULE 4:blockVariable can be used only in this block.
		    int blockVariable;
		    //Some Code
		}

		//blockVariable = 5;//COMPILER ERROR - RULE 4
    }
    
    void method2() {
		//method1LocalVariable = 5; //COMPILER ERROR - RULE3
    }
    
    static void staticMethod() {
		staticVariable = 5;//RULE 1
		//memberVariable = 5; //COMPILER ERROR - RULE 2
    }
}
```

#### Scope Example 1
- staticVariable is declared using keyword static. 
- It is available in the instance method method1 and static method named staticMethod.

#### Scope Example 2
- memberVariable is declared directly in the class  and does NOT use keyword static. So, it is an instance variable. 
- It is available in the instance method method1 but not accessible in the static method named staticMethod.

#### Scope Example 3
- method1LocalVariable is declared in the method method1. So, it is a local variable. 
- It is available in the instance method method1 but available in any other  instance or static methods.

#### Scope Example 4
- blockVariable is declared in a block in method1. So, it is a block variable. 
- It is available only in the block where it is defined. 
- It is not accessible any where out side the block , even in the same method.

### Variable Initialization
- Initialization defines the default value assigned to a variable if it is not initialized.

#### Important Rules
- Member/Static variables are alway initialized with default values.
- Default values for numeric types is 0, floating point types is 0.0, boolean is false, char  is '\u0000' and for a object reference variable is null.
- Local variables are not initialized by default by compiler. 
- Using a local variable before initialization results in a compilation error.
- Assigning a null value is a valid initialization for reference variable



