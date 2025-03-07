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

[Watch this video:](https://youtu.be/7yr81Dnn0NY?si=a5Yc6NEeBfCkoqlT) for more details.

<br>

![zp](https://github.com/user-attachments/assets/f30c99df-1027-47b1-8beb-2f93aa558c51)

<br>

## Java Architecture:

| Architecture of Java | Execution of Java |
|---------|---------|
|![image](https://github.com/user-attachments/assets/3a28630b-7162-4102-846f-110b0507cee6) | ![ezgif-69eb78587e90da](https://github.com/user-attachments/assets/33d2117e-2331-48a9-94c5-92a42bb2ddc2)|

<br>

## Java Environment Components  

## 1. JDK (Java Development Kit)  
Java Development Kit provides the environment to develop and execute Java programs. It includes:  
- A **compiler**, an **archiver**, a **debugger**, and other development tools.  
- **Java Runtime Environment (JRE)** for executing Java programs.  

**Note:** 
`JDK is platform-dependent, so separate installers are needed for Windows, Unix, and Mac operating systems.`

JDK mainly includes two components:  
- **Development Tools** – Provides an environment to develop Java programs.  
- **JRE** – Used to execute Java programs.

<br>

## 2. JRE (Java Runtime Environment)  
Java Runtime Environment is a software package that provides an environment to **run** Java programs (not develop them).  

It contains:  
- **JVM (Java Virtual Machine)**  
- **Libraries and Other Components** required to run Java applications.  

**Note:** 
 `JRE is platform-dependent`
 `JRE is primarily for running Java applications, not for development.`
 
<br>

## 3. JVM (Java Virtual Machine)  
JVM is a virtual CPU that provides a runtime environment for executing Java bytecodes.  

It performs the following tasks:  
- Converts **bytecode** into **machine-specific code**.  
- Loads class files in the **class loader**.  
- Verifies bytecode with the **bytecode verifier**.  
- Executes bytecode line by line (hence, it acts as an **interpreter**).  

**Note:** 
`JVM is platform-Independent`

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

## Architecture of JDK, JRE, JVM:

![image](https://github.com/user-attachments/assets/f892ba83-e9d9-4cc5-adeb-9c96d9cd7f59)

<br>

## First Java Program

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

## Can We Perform Changes in Bytecode? 
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

## Size of Data Type in Java

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

#### 1. `byte b33 = 128;`
- **Error**: `128` is outside the range of the `byte` data type, which can only hold values from `-128` to `127`.

#### 2. `byte b44 = -129;`
- **Error**: `-129` is also outside the range of the `byte` data type.

#### 3. `int i13 = 2147483648;`
- **Error**: `2147483648` is out of range for the `int` type, which supports values from `-2147483648` to `2147483647`.

#### 4. `long l14 = 2147483649;`
- **Error**: Although `2147483649` fits within the `long` range, it is treated as an `int` by default in Java. Adding an `L` at the end like `2147483648L` tells the compiler to treat it as a `long`.

#### 5. `float f11 = 11.11;`
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

#### `print` and `println` and `printf`

- `print()`: Outputs text on the same line.
- `println()`: Outputs text and then moves to the next line.
- Printf(): Outputs formatted output to the console.

#### Format/Printf Examples
Let's look at a few examples to quickly understand printf function. 
```java
System.out.printf("%d", 5);//5
System.out.printf("My name is %s", "Rithu");//My name is Rithu
System.out.printf("%s is %d Years old", "Rithu", 5);//Rithu is 5 Years old
```
In the simplest form, string to be formatted starts with % followed by conversion indicator => b - boolean c - char d - integer f - floating point s - string.
<br>

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
<br>

## Scanner Class
- The Scanner class is a predefined class in Java used for reading input from various sources, such as the keyboard (System.in), files, or strings. It enables programs to accept user input at runtime, making applications interactive.
- To use the Scanner class, you first need to import it from the `java.util` package. 
- The Scanner class provides various methods to read different types of input. Some commonly used methods include:

- `nextByte()`: Reads a byte value.

- `nextBoolean()`: Reads a boolean value (true/false).

- `nextShort()`: Reads a short integer.

- `nextInt()`: Reads an integer.

- `nextFloat()`: Reads a float value.

- `nextDouble()`: Reads a double value.

- `nextLong()`: Reads a long integer.

- `next()`: Reads a single word (string without spaces).

- `nextLine()`: Reads a whole line (string with spaces).

## Important Notes:
- **InputMismatchException:** If the user provides an input of a type that doesn’t match the expected type, a java.util.InputMismatchException will be thrown.
 ``` For example, if you enter a float when an integer is expected:
Enter age:  44.5
Exception in thread "main" java.util.InputMismatchException
```
-**No nextChar() Method:** There is no method named nextChar(). Instead, to get a character input, you can read a string using next() and then use charAt(index) to retrieve the desired character.

<br>

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
  
<br>

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
<br>

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

float f = 123.456; //COMPILER ERROR! A double value cannot be assigned to a float.

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
    
![image](https://github.com/user-attachments/assets/c20b4abf-1fd3-4b14-a1b2-146644f6a73c)


## Q. What is Operand and Operator
- The values or variables on which the operator acts on it is known as Operand. Eg:a,b
- Operator is a symbol or keyword used to perform operations on operands Eg: +
```
int c=a+b;
```
## Q. What is Field and Attributes
- Field-> A variable with values is known as field
- Attributes->The name of the variable.

<br>

## Control Statements in Java

## If-Else Statement
The `if-else` statement controls the execution of code blocks based on whether a condition evaluates to `true` or `false`.

```java
if (condition) {
    // Code executes if condition is true
} else {
    // Code executes if condition is false
}
```
## Nested If Statement

- You can place an if statement inside another if to create complex decision-making scenarios.
```java
if (condition1) {
    if (condition2) {
        // code if both condition1 and condition2 are true
    }
}
```
## If-Else Ladder

- Multiple if-else statements chained together. Useful when you need to test several conditions.

```java
if (condition1) {
    // code if condition1 is true
} else if (condition2) {
    // code if condition2 is true
} else {
    // code if none of the above are true
}
```
<br>

## Loops
Loops facilitate the execution of a set of instructions repeatedly until a specific condition is met.

### 1. While Loop
Executes repeatedly until the specified condition becomes `false`.

```java
while (condition) {
    // Code executes while condition is true
}
```

### 2. Do-While Loop
Executes the block at least once before checking the condition, then repeats as long as the condition is `true`.

```java
do {
    // Code executes at least once
} while (condition);
```

### 3. For Loop
Used when the number of iterations is known beforehand. It consists of three parts: initialization, condition, and increment/decrement.

#### Normal For Loop:
```java
for (int i = 0; i < 5; i++) {
    System.out.println(i);
}
```

#### Enhanced For Loop:
Used to iterate through arrays and collections in Java. It starts with index `0`.

```java
String[] cars = {"Volvo", "BMW", "Ford", "Mazda"};
for (String car : cars) {
    System.out.println(car);
}
```
**Note:** Printing `car` gives the values of the array, whereas printing `cars` prints the memory location of the array.

#### Nested For Loop:
Used for iterating through rows and columns, commonly used in 2D structures and nested iterations.

```java
// Outer loop
for (int i = 1; i <= 3; i++) {
    // Inner loop
    for (int j = 1; j <= i; j++) {
        System.out.println("Inner: " + j);
    }
}
```
**Execution Flow:**
- When `i = 1`, `j` runs for `1`.
- When `i = 2`, `j` runs for `1, 2`.
- When `i = 3`, `j` runs for `1, 2, 3`.

<br>


## Switch Statement
- The `switch` statement selects one block from multiple blocks to e executed based on a matching value.
- Multiple nested `switch` statements can also be used.
**Note:**
- For `char`, use single quotes (`'A'`).
- For `String`, use double quotes (`"Hello"`).
- Disallowed Types:
- float, double, long: These types are not allowed in a switch statement.
- boolean: The boolean type cannot be used in a switch statement.
```java
int number = 2;
switch (number) {
    case 1:
        System.out.println("One");
        break;
    case 2:
        System.out.println("Two");
        break;
    default:
        System.out.println("Not One or Two");
}
```

`Nested switch:`
```java
public class NestedSwitchExample {
    public static void main(String[] args) {
        String day = "Monday";
        String topic = "Collections";

        switch (day) {
            case "Monday":
                System.out.println("Start of the week");

                switch (topic) {
                    case "Collections":
                        System.out.println("Today's topic: Learning Java Collections");
                        break;
                    case "OOP":
                        System.out.println("Today's topic: Learning Object-Oriented Programming");
                        break;
                    default:
                        System.out.println("General Java learning session");
                }
                break;

            case "Friday":
                System.out.println("End of the week");
                break;

            default:
                System.out.println("Midweek day");
        }
    }
}
```
<br>

## Enums in Java
An `enum` (enumeration) is a special class that represents a group of constant values and it is known at compile time.
### Enum Methods
- To access a single value of an `enum`, use `enum_name.valueOf()`
- To directly access a particular value, use `enum_name.valueName`.
- To access all values of an `enum`, use `enum_name.values()`.

```java
enum Color { RED, GREEN, BLUE }
Color color = Color.RED;
switch (color) {
    case RED:
        System.out.println("Red color");
        break;
    case GREEN:
        System.out.println("Green color");
        break;
}

enum courses { JAVA, AI, ML }
courses selectedCourse = courses.valueOf(a);
switch (selectedCourse) {
      case JAVA:
           System.out.println("Java course");
           break;
      case AI:
           System.out.println("AI course");
	   break;
      case ML:
	   System.out.println("MI course");
           break;
      default:
           System.out.println("Invalid course");
     }
}}
```

<br>

## Type Casting in Java

- Type casting is a concept in programming where you change the data type of a variable from one type to another.

- In Java, there are two types of casting:

## 1. Implicit Casting (Automatic)
- Also known as widening casting
- **automatically** when converting a smaller type to a larger type.
- Order: byte -> short -> char -> int -> long -> float -> double
```java
public class ImplicitCastingExample {
    public static void main(String[] args) {
        int myInt = 10;
        double myDouble = myInt; // Implicit casting from int to double
        System.out.println("Integer value: " + myInt); // Outputs: Integer value: 10
        System.out.println("Double value: " + myDouble); // Outputs: Double value: 10.0
    }
}
```

## 2.Explicit Casting (manually) 
- Also known as Narrowing Casting
- **manually**Converting a larger type to a smaller size type
- Order:double -> float -> long -> int -> char -> short -> byte
```java
public class NarrowingCastingExample {
    public static void main(String[] args) {
        double myDouble = 9.78;
        int myInt = (int) myDouble; // Explicit casting from double to int
        System.out.println("Double value: " + myDouble); // Outputs: Double value: 9.78
        System.out.println("Integer value: " + myInt); // Outputs: Integer value: 9
    }
}
```
<br>

## Wrapper Classes
- Wrapper classes provide a way to use primitive data types (int, float,boolean etc..) as objects. 

## Need of Wrapper Classes
- Data structures in the Collection framework, such as ArrayList and Vector, store only objects (reference types) and not primitive types.

## 1.Autoboxing
- Autoboxing is the automatic conversion of a primitive type to its corresponding wrapper class object. For example – conversion of int to Integer, long to Long, double to Double, etc.
  
## 2. Unboxing
- Unboxing is the automatic conversion of a wrapper class object to its corresponding primitive type. It is just the reverse process of autoboxing. For example – conversion of Integer to int, Long to long, Double to double, etc.

```java
public class Wrapperclasses {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		//Boxing or Wrapping
		int obj=10;
		Integer a=Integer.valueOf(obj);
		int j=a.intValue();//UnBoxing
		
		
		byte b=10;
		long l=123456;
		short s=4;
		double d=55.98D;
		boolean b2=true;
		float f=67.987F;
		int i=76;
		char c='a';
		
		//autoboxing: Converting primitive to objects
		Byte byteobj=b;
		Long longobj=l;
		Short shortobj=s;
		Double doubleobj=d;
		Boolean booleanobj=b2;
		Float floatobj=f;
		Integer intobj=i;
		Character charobj=c;
		System.out.println("Primitive type to Object:");
		System.out.println("--------------------------------");
		
		//Autounboxing: convert objects to primitive
		
		byte bytevalue=byteobj;
		long longvalue=longobj;
		short shortvalue= shortobj;
		double doublevalue=doubleobj;
		boolean booleanvalue=booleanobj;
		float floatvalue=floatobj;
		int intvalue= intobj;
		char charvalue= charobj;
		
		System.out.println("Objects to primitives:");
		System.out.println("--------------------------------");
		
		//Converting String into datatype [String itself comes under Object an instance of the String class.]
		System.out.println("String to primitives");
		String s1="123";
		int val=Integer.parseInt(s1);
		System.out.println(val);
		String s2="10";
		double val2=Double.parseDouble(s2);
		System.out.println(val2);

	}

}
``` 

## Wrapper Class Utility Methods

- A number of utility methods are defined in wrapper classes to create and convert them.

#### valueOf  Methods
We can use the valueOf() method to create a Wrapper object for a given primitive or String. 

>  Wrapper valueOf(String s): 
> >Every wrapper class except Character class contains a static valueOf() method to create Wrapper class object for a given String.

``` java
class GFG { 
	public static void main(String[] args) 
	{ 
		Integer I = Integer.valueOf("10"); 
		System.out.println(I); 
		
		Double D = Double.valueOf("10.0"); 
		System.out.println(D); 
		
		Boolean B = Boolean.valueOf("true"); 
		System.out.println(B); 

		// Here we will get RuntimeException 
		Integer I1 = Integer.valueOf("ten"); 
	} 
}
```

> Wrapper valueOf(primitive p):
> > Every Wrapper class including the Character class contains the following method to create a Wrapper object for the given primitive type.

```java
// Java program to illustrate valueof() Method 

class GFG { 
	public static void main(String[] args) 
	{ 
		Integer I = Integer.valueOf(10); 
		Double D = Double.valueOf(10.5); 
		Character C = Character.valueOf('a');
                Boolean B = Boolean.valueOf("true"); 
		System.out.println(B); 
		System.out.println(I); 
		System.out.println(D); 
		System.out.println(C); 
	} 
}
```

#### xxxValue methods 

We can use xxxValue() methods to get the primitive for the given Wrapper Object.
```java
Integer integer = Integer.valueOf(57);
int primitive = integer.intValue();//57
float primitiveFloat = integer.floatValue();//57.0f

Float floatWrapper = Float.valueOf(57.0f);
int floatToInt = floatWrapper.intValue();//57
float floatToFloat = floatWrapper.floatValue();//57.0f
```

#### parseXxx methods

We can use parseXxx() methods to convert String to primitive. 

```java
// Java program to illustrate parseXxx() Method 

class GFG { 
	public static void main(String[] args) 
	{ 
		int i = Integer.parseInt("10"); 
		double d = Double.parseDouble("10.5"); 
		boolean b = Boolean.parseBoolean("true"); 
		
		System.out.println(i); 
		System.out.println(d); 
		System.out.println(b); 
	} 
}
```
#### toString() Method
We can use the toString() method to convert the Wrapper object or primitive or any other to String.

```java
// Java program to illustrate toString() Method 

class GFG { 
	public static void main(String[] args) 
	{ 
		Integer I = new Integer(10); 
		String s = I.toString(); 
		System.out.println(s); 
	} 
}
```
<br>

## Variables in Java

###  Instance Variable vs. Static Variable vs. Local Variable

| Feature                | Instance Variable | Static Variable | Local Variable |
|------------------------|------------------|----------------|---------------|
| Defintion |An **instance variable** is a variable that belongs to an object (instance) of a class. It is declared inside a class but outside any method. |A **static variable** is a class-level variable which is shared among all instances of the class. It is declared using the `static` keyword.| variables are declared within a method, constructor, or block.They must be initialized before use, as they do not have default values.|
| Memory Allocation      | Created when an object is instantiated. | Allocated once when the class is loaded. | Allocated when the method/block is executed and destroyed after execution. |
| Memory Location      | Located in Heap | Located in Heap  | Located in Stack |
| Scope                 | Specific to each object. | Shared across all objects of the class. | Limited to the method/block in which it is declared. |
| Default Values        | Assigned default values by JVM. | Assigned default values by JVM. | Must be explicitly initialized before use. |
| Access in Static Methods | Cannot be accessed directly in a static method. | Can be accessed directly in static and non-static methods. | Cannot be accessed outside the method/block. |
| Access in Non-Static Methods | Can be accessed directly in non-static methods. | Can be accessed directly in both static and non-static methods. | Can only be accessed within the method/block where declared. |
| Modifiers Allowed | Can use all access modifiers. | Can use all access modifiers. | Can only be `default` or `final` (cannot be `private`, `public`, or `protected`). |


<br>

## Question based on variables

### Q. Is Initialization of Local Variables Mandatory?
**Yes**, it is mandatory to initialize local variables. If we do not initialize them, we will get a compile-time error saying:
```
Variable might not be initialized
```

### Q. What if local variable and global variable names are same?
- If local var and global var names are same first priority is always given to local variables because they are inside method and nearer for execution to JVM.

### Can we directly use static variables inside the main?
-	No, we can’t use the static variables inside the main without a method.

### Can we mark a local variable as static?
- No, we cannot mark a local variable with a static keyword.

### How to access static variables without using methods?
- By directly printing the name of the variables

### Can we call a static variable by using objects?
- Yes, we can call a static variable directly by using object but it’s called object cloning and we should not call static variable by using object.

### Diff b\w null and 0’s 
- 0 is value and null is nothing where we create an empty memory	

<br>

# Methods

## Overview
- A method is a block of code that only runs when it is called.
- We can pass parameters to a method.
- Methods are similar to functions in C++ and Python.

## Use of Methods
- Define once and use it many times.
<br>

## Method Return Type:

The return type of a method indicates what type of value it will return to the caller:

- Primitive types: The method can return values like int, float, boolean, etc.

- Reference types: The method can return objects, arrays, or user-defined types.

- Void: If a method has a void return type, it does not return any value.
<br>

## Memory Management of Methods:

- When a method is invoked, it gets memory allocated in the stack area as a stack frame.

- The method’s stack frame is created when the method is called and released once it completes execution.

- Java stack follows the Last-In-First-Out (LIFO) principle, meaning the last method invoked will be the first to complete.
<br>

## Static Methods:
- Static Methods are methods that are associated with the class not with objects of the class
- For Static Methods, we can able to pass the arguments with class_name.method_name without creating objects.
<br>

## Method Overloading
- Multiple methods can have the same name with different parameters or different data types.
- Example: Amazon payment portal (By UPI, Netbanking, Credit Cards, Amazon Pay Balance).
- Also called:
  - Function Overloading
  - Compile-time Polymorphism
  - Static Polymorphism
  - Early Binding Polymorphism

### How to Perform Method Overloading?
- By changing the number of parameters.
- By changing the data type.
- By changing the order of parameters.

<br>

## Method Overriding
- A subclass (child class) can access the same method of a parent class.
- Also called:
  - Run-time Polymorphism
- **IS-A** relationship is mandatory to perform overriding.
- While overriding, the method name and arguments must be the same.
- Example: Updating an existing feature.
### Note:
- Private,static and final methods cannot be overriden.

 ## Method Chaining:
- Method chaining refers to calling multiple methods sequentially within another method
<br>

## Difference b/w Method Overloading and Method Overriding

| Feature                                | Method Overloading                                      | Method Overriding                                       |
|----------------------------------------|---------------------------------------------------------|---------------------------------------------------------|
| Purpose                                | Increases readability of the program                   | Provides a specific implementation of a superclass method |
| Implementation                     | Within a single class                                   | In two classes with an IS-A (inheritance) relationship |
| Parameter requirement                   | Must be different                                      | Must be the same                                       |
| Type of polymorphism                   | Compile-time polymorphism                              | Run-time polymorphism                                  |
| Return type condition                   | Cannot be overloaded by changing only return type; parameters must change | Return type must be the same or covariant|
| Error detection                         | Errors can be caught at compile-time                  | Errors are caught at run-time                          |
| Applicability to private & final methods | Applicable                                            | Not applicable                                        |                         
| Static methods                          | Can be overloaded                                     | Cannot be overridden                                  |

<br>

## Questions based on Methods

### Q. Can we overload final methods ?
 Yes, we can overload final methods because final keyword says do not
change implementation and in overloading we are not changing
implementation rather we are changing arguments.

### Can we overload private methods or not ?
A. Yes, we can overload private methods because private methods are
accessible everywhere in same class and overloading also happens within
class.

### Can we overload non static methods or not ?
A. Yes, we can overload non static methods but to call them we have to
create an Object.

### Can the Main Method be Overloaded?
- Yes, we can overload the `main` method in Java, but JVM only calls the original `main` method. It will never call our overloaded `main` method.
  
```java
public class CanMainbeOverloaded {
	public static void main(String[] args) {
		System.out.println("Original Main Method");
	}
	
	public static void main(Double[] args) {
		System.out.println("Overloaded Main Method");
	}
	
	public static void main(int args) {
		System.out.println("Overloaded Main Method");
	}
}
```

- **Output:** `Original Main Method`

### Can the Main Method be Overridden?
- No, we cannot override the `main` method in Java because a static method cannot be overridden.

### Can we call the main method explicitly?
- Yes we can call  the main Method Explicitly.
```java
public class MainExample {
    public static void main(String[] args) {
        System.out.println("Main method called");
    }
    public static void anotherMethod() {
        main(new String[]{"arg1", "arg2"}); // Calling main explicitly
    }
    public static void main(String[] args) {
        anotherMethod();
    }
}
```

### Can We Pass an Object Inside Method Calling?
- Yes, you can pass objects as parameters inside a method.
- Any changes made to the object in the called method will be reflected in the calling method as well.
  
```java
public class CanWePassObjectsinMethodCall {
	int b=20;
	void mc(int a) {
		System.out.println("Passing Objects in method call: "+a);
	}
	public static void main(String[] args) {
		// TODO Auto-generated method stub
		CanWePassObjectsinMethodCall obj=new CanWePassObjectsinMethodCall();
		obj.mc(obj.b);//passing object in method call
	}
}
```

### Can we overload static methods? 
- Yes. We can have two or more static methods with the same name, but parameters or datatypes should be different.

### Can we overload methods that differ only by static keywords? 
- We cannot overload two methods in Java if they differ only by static keyword (the number of parameters and types of parameters is the same).
```java
public class Test {
	public static void foo() {
		System.out.println("Test.foo() called ");
	}
	public void foo() { // Compiler Error: cannot redefine foo()
		System.out.println("Test.foo(int) called ");
	}
	public static void main(String args[]) { 
		Test.foo();
	}
}
```
<br>

### Call by Value:
- Calling a method by passing a value in the parameter.
- Any changes made to the parameter within the method doesn’t affect the original value outside the method.
```java
public class CallByValue {
	int data=50;//instance variable
	void print(int data){ //cpy of data is passed to the method (localvariable)
		data=data+100; //changes in local variable only it won't affect the original variable outside the method.
	}
	
	public static void main(String[] args) {
		// TODO Auto-generated method stub
		CallByValue obj=new CallByValue();
		System.out.println("Before Change: "+obj.data);//calling instance variable
		obj.print(500);//calling method
		System.out.println("After Change: "+obj.data);
	}
 }
```
[CallbyValue Explanation](callbyvalue.pdf)


**NOTE**: `Java doesn't have CallByReference because java doesn't support pointers.`

<br>

# Variable Arguments (Var-Args)

## Overview
- Variable Arguments, commonly known as var-args, allow methods to accept multiple arguments of a specified type.
- Make methods more flexible and no need of overloaded methods
- Java will pack args into array format
```
 Syntax:
- The syntax of a variable argument is <data_type> … <var_name>.
- Example: int… nums or String… words.
```

### Key Rules:
- **One Var-Args per Method:** You can only have one var-args parameter in a method.
- **Var-Args must be the Last Parameter:** If combined with other parameters, the var-args parameter must always appear at the end.

## Example of Var-Args Usage

```java
public class VarArgs {
	public static void varargs(String... strval) {
		for (String a : strval) {
			System.out.println(a);
		}
	}

	public static void main(String[] args) {
		VarArgs.varargs("Hari", "Dinesh", "Kumar", "Saran","Rohit");
	}

}
```

## Combining Var-Args with Regular Parameters
You can combine regular parameters and var-args in a method, but the var-args parameter must always be the last parameter.

### Example:
```java
public class VarArgs {
    public static void varargs(int num, String... values) {
        System.out.println("Fixed Number: " + num);
        for (String val : values) {
            System.out.println(val);
        }
    }

    public static void main(String[] args) {
        VarArgs.varargs(5, "Hari", "Dinesh", "Kumar", "Saran", "Rohit");
    }
}

```
<br> 


# Java Constructors

## Overview

- Constructor is a special method that is used to initialize the objects.
- By default, a constructor is called when an object is created.
- It can be used to set initial values for object attributes.
- A constructor in Java can’t be abstract, final, static, or synchronized.
- Same Name as Class Name
- No return Type
- Automatic invocation (e.g., if we apply brakes, the car will stop).
- Initialization of objects

<br>

## How Java Constructors are Different from Methods?

| Feature            | Constructors | Methods |
|--------------------|-------------|---------|
| Name              | Must be the same as the class name | Can have different names |
| Return Type       | No return type | Has a return type or `void` if it does not return any value |
| Invocation        | Called only once at the time of object creation | Can be called any number of times 

<br>

## Types of Constructors

### 1. Default Constructor
A constructor that has no parameters is known as a default constructor. The default constructor provides default values to the object like `0`, `null`, etc., depending on the type.

### 2. Parameterized Constructor
A constructor that allows us to pass one or more arguments. It is used to initialize the object's properties with specific values (if we want to initialize variables with our own values).

### 3. Copy Constructor
A constructor that is used to create a new object by copying values from an existing object of the same class.
> **Note:** Java does not support copy constructors, but they can be implemented manually.
<br>

## Constructor Overloading

-  Constructor overloading is a technique of having more than one constructor in the same class with different parameter lists.

- Constructor overloading allows multiple ways to initialize an object.
  
```java
public class Person 
{	
// Declaring a non-parameterized constructor.
   Person() { 
      System.out.println("Introduction:");
   }
// Declaring one parameterized constructor.
   Person(String name){
     System.out.println("Name: " +name);	
   }
// Declaring two parameterized constructor.
   Person(String scname, int rollNo) {
	 System.out.println("School name: "+scname+ ", "+"Roll no:"+rollNo);
   }
public static void main(String[] args) 
{
 // JVM will call constructor depending on arguments passed.
  Person p1 = new Person(); // calling with zero argument.
  Person p2 = new Person("John"); // calling with one argument.
  Person p3 = new Person("DPS", 12); // calling with two arguments.
 }
}
```
<br>

## Constructor Chaining

- Constructor chaining occurs when one constructor calls another constructor in the same class using this()
- Rules for Constructor Chaining:
> 1. this() must be the first statement in the constructor.
> 2. Only one constructor call is allowed in each constructor.

```java
class A {
    A() {
        System.out.println("No-parameter constructor in A class");
    }
    
    A(int a) {
        this();  // Calls the no-parameter constructor
        System.out.println("1-parameter constructor in A class");
    }
    A(int a, int b) {
        this(a);  // Calls the 1-parameter constructor
        System.out.println("2-parameter constructor in A class");
    }
}
class ConstructorChaining {
    public static void main(String[] args) {
        A a1 = new A(10, 20);  // Invokes the 2-parameter constructor
    }
}
```

### Q What is Constructor calling?
- The process of calling one constructor from another constructor within the same class is known as Constructor calling.

### Q Can a Constructor can be static,final or abstract?
- **No** , A Constructor cannot be static or final or abstract
  
###  Q Can a Constructor can be public,private or protected?
- **Yes**, a Constructor can be public or private or protected
<br> 

# Object-Oriented Programming Concepts

## Class:
- A Class is a blueprint or template or user-defined prototype for creating objects.
- It consists of Data members, methods, constructors, nested classes, interfaces etc.
  
## Object: 
- Objects is a real time entity and it’s created at run time.
- It is known as instance of a class
- Each object has a state, behaviour, identity.
- The objects can be created by using the new keyword.
- Default value of Object is null
  
![image](https://github.com/user-attachments/assets/5bcefa1a-754d-403d-9be6-4f85a4183d22)
- State: It is represented by attributes(variables) of an object. 
- Behaviour: It is represented by the methods of an object.
- Identity: It gives a unique name to an object.

- More info:(https://www.geeksforgeeks.org/reference-variable-in-java/)


# Object-Oriented Programming System (OOPs)

## Overview

- Object-Oriented Programming System (OOPs) is a programming concept based on objects. 
- It provides a structured way to design and develop software using principles like Encapsulation, Abstraction, Inheritance, and Polymorphism.

## Why Do We Need OOP?

- **Organized Code** – Helps structure programs neatly.
- **Reusability** – Write code once, use it multiple times.
- **Security** – Protects important data from unwanted changes.
- **Scalability** – Makes it easy to expand projects without breaking existing code.
<br>

## Inheritance in OOP

Inheritance is an OOP concept that allows a class to inherit properties and behaviors from another class.
**Example:** A child inherits some properties from their parents.

### How is inheritance implemented in Java?
Inheritance is implemented using the `extends` keyword.

### Superclass
The class whose features are inherited is known as the **superclass**, **base class**, or **parent class**.

### Subclass
The class that inherits from another class is called the **subclass**, **derived class**, **extended class**, or **child class**.

## Importance of Inheritance in Java

- **Reusability**: The major advantage of inheritance is code reuse.
- **Extendibility**: We can add new functionality to our application without modifying existing code.
- Example: Microsoft Word has multiple versions such as Word 2003, 2007, etc. Instead of rewriting the entire code, the existing code is reused with additional features.
<br>

### Types:
![image](https://github.com/user-attachments/assets/1467fe72-5bd4-4e3d-83c0-38fbb62f7c60)

### Single Inheritance: 
- One class that is allowed to inherit the immediate child class or parent class 
- Example: Father → Son
``` java
//constructor-super-ovveride
class Credentials {
	public int regno;
	public String psw;

	Credentials(int regno, String psw) {
		this.regno = regno;
		this.psw = psw;
	}

	public String display(int regno, String psw) {
		return ("The credentials are " + regno + " " + psw);
	}
}

class Profile extends Credentials {
	public String name;
	public String dept;

	Profile(int regno, String psw, String n, String dt) {
		super(regno, psw);
		name = n;
		dept = dt;
	}

//over-ride
	public String display() {
		return (super.display(regno, psw) + " and the profile is " + name + " from " + dept);
	}
}

public class T_Singleinheritance {
	public static void main(String[] args) {
		// TODO Auto-generated method stub
		Profile obj = new Profile(21500169, "8C1l1", "Hariharan", "IT");
		System.out.println(obj.display());

	}

}

```
<br>

### Multilevel Inheritance: 
- It is a chain of inheritance Where one class inherits from another class, and then another class inherits from it.
- Example: Grandparent → Parent → Child
``` java
//skeleton class
class shape//super class
{
	public void display() {
		System.out.println("Inside shape method");
	}
}

class rectangle extends shape //subclass1
{
	public void area() {

		System.out.println("Inside rectangle method");
	}
	
}
class cube extends rectangle//subclass2
{
	public void volume() {

		System.out.println("Inside cube method");
	}
}

//stub class
public class MultilevelInheritance {
	public static void main(String[] args) {
		// TODO Auto-generated method stub
		cube c =new cube();// all the features will come in cube(including shape,rect.
		c.display();
		c.area();
		c.volume();

	}

}

```
<br>

### Hierarchical Inheritance:   
- Multiple classes to inherit from a single parent class.
- Example: SCOFT->IT, CSE, AIDS
``` java
class departments{
	String depts="SCOFT";
}
class department1 extends departments{
	String dept1="IT";
}
class department2 extends departments{
	String dept2="CSE";
}
class department3 extends departments{
	String dept3="AIDS"; 
}
class department4 extends departments{
	String dept4="ECE"; 
}

public class T_Hierarchalinheritance {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		department1 obj1=new department1();
		department2 obj2=new department2();
		department3 obj3=new department3();
		department4 obj4=new department4();
		
		System.out.println(obj1.dept1+" The dept is under "+ obj1.depts);
		System.out.println(obj2.dept2+" The dept is under "+ obj2.depts);
		System.out.println(obj3.dept3+" The dept is under "+ obj1.depts);
		System.out.println(obj4.dept4+" The dept is under "+ obj1.depts);
		
```
<br>

### Hybrid Inheritance: 
- Hybrid is a combination of two or more types of inheritance in a class Hierarchy.
- Single, multilevel, hierarchical can be used in this inheritance.
``` java
class grandfather{
	public void showG() {
		System.out.println("He is a grand father");
	}
}
class father extends grandfather{
	public void showF() {
		System.out.println("He is a father");
	}
}
class son extends father{
	public void showS() {
		System.out.println("He is a Son");
	}
}

public class HybridInheritance extends father// if we put son it will only give son and inherited things
{
	public void showD() {
		System.out.println("She is a Daughter");
	}
	public static void main(String[] args) {
		// TODO Auto-generated method stub
		son obj1=new son();
		obj1.showS();
		obj1.showF();
		obj1.showG();
		System.out.println("-----------------------------");
		HybridInheritance obj2=new HybridInheritance();
		obj1.showS();
		obj2.showD();
		obj2.showF();
		obj2.showG();

	}

}
```
<br>

### Multiple Inheritance: 
- A class that can inherit properties of more than one parent class.
  
### Java doesn’t support Multiple Inheritance Why? 
- As per java rule whenever we create an object for subclass object its super class constructor must be executed first in-order to complete the constructor chaining process
- This is because a subclass inherits properties from its superclass, and before the subclass can use them, the superclass must be properly initialized.
- In multiple inheritance, a subclass has more than one superclass. That means if Java allowed multiple inheritance, a subclass would have two or more superclass constructors to call.
- So, the JVM will get confuse constructor should be called first to complete the constructor chaining.
- To avoid this confusion multiple inheritance is not allowed in java.

<br>
  
### Q. Can we access all variables and features of parent class in child class?
- No, the accessibility of parent class features inside child class is also decided by access modifier. For example, a private variable or method in parent class won't be accessible inside child class.

### Q.What do you do if you don’t want a class to be inherited?
- Just make it final
  
<br>

## this Keyword
- ‘this’ keyword in Java is a reference variable that refers to the current instance of the class. It is commonly used to differentiate between instance variables and method parameters with the same name.
- this can also be used to:
- Call current class constructor
- Call current class method
- to refer to the current class instance variables.

<br>

##  Super Keyword
- Super is a keyword that reference parent class or super class or subclass in java (it only returns parent object) it return the objects that represents from parent class
- super can be used in various contexts as given below:
- it can be used to refer superclass instance variable
- it can be used to call a superclass method
- it can be used to call a superclass constructor.
  
<br>

## Similarities
- `this()` and `super()` must be the first statements in a constructor.
- Both this and super are non-static, so they can't be used in static context. It means that we cannot use both the keywords in the main method in Java.
- Both super and this keywords in Java can be used in constructor chaining to call another constructor. this() calls the no-argument constructor of the current class, and super() calls the no-argument constructor of the parent class.
- 
<br>

## Interview Question: When Do You Need a `super` Keyword?

- Whenever a sub class inherits the features of a super class, there is a chance that super class features are similar to derived sub features, resulting in ambiguity for the JVM. The `super` keyword must be used to distinguish between base class features and derived class features.

## Can We Use Both `this()` and `super()` in the Same Constructor?

- No, Both this() and super() cannot be used together in constructor.
- this() is used to call default constructor of same class.it should be first statement inside constructor.
- super() is used to call default constructor of base class.it should be first statement inside constructor.
- so this() and super() both are used for constructor call but both want to execute at first. that's why it'll show compiler error like :
```java
error: call to this must be first statement in constructor this(); or

error: call to this must be first statement in constructor super();
```

```java
public Animal() {
    this.name = "Default Name";
    //super(), if called, should always the first statement in a constructor.
    //super(); //COMPILER ERROR
}

public Animal() {
    System.out.println("Creating an Animal");
    //this(string), if called, should always the first statement in a constructor.
    //this("Default Name");//COMPILER ERROR
}
```
<br>

# Coupling in Java

Coupling in Java refers to the degree of interdependence between different modules or classes in a software system. It measures how closely classes or components are connected. In a well-designed software system, it's generally desirable to have **low coupling**. This promotes modularity, reusability, and maintainability.
<br>

## Types of Coupling in Java

### Loose Coupling
Loose coupling in Java refers to designing classes and components in a way that minimizes their interdependence. In a loosely coupled system, classes or modules are independent, meaning that changes in one module do not require changes in other modules. This promotes modularity, ease of maintenance, and code reusability.

### Tight Coupling
Tight coupling in Java refers to a situation where classes or modules are highly interdependent, meaning that changes in one module often require changes in other modules. Tight coupling can lead to code that is difficult to maintain, as modifications in one part of the system can inadvertently affect other parts.

![image](https://github.com/user-attachments/assets/25aa624a-610a-4c52-8153-a4748495551a)

<br>

## Abstraction
Abstraction is the process of hiding the implementation details and only showing the essential functionality or features to the user.  

### Real-time Example
When you get a call, we get an option to either pick it up or just reject it. But in reality, there is a lot of code that runs in the background.

### Two Ways to Achieve Abstraction:
- **Abstract class (0 to 100%)**
- **Interfaces (100%)**

### Abstract Class
An abstract class is a restricted class that cannot be used to create objects. It can only be inherited and accessed from another class.

- `abstract` method can be used in an abstract class and doesn't have a body (declaration). The body (definition) should be provided by the subclass.
- An abstract class must contain at least one abstract method.
- We can also use abstract and normal methods in an abstract class.
- We must define concrete methods in an abstract class otherwise it will raise an error.
- We can indirectly create objects for abstract classes by extending them.
 ```java
abstract class animal
{
	public abstract void animalsound();// abstract method?[methods having only declaration. (Body of the method should be in sub class only)]
	public void sleep() 
//regular method or concrete method (we must define it otherwise it will raise error)
	{
		System.out.println("Sleep");
	}
	
}
class pig extends animal//sub-class
{
	 public void animalsound() {
		System.out.println("weee-weee");
	}
}


public class AbstractClass {
	public static void main(String[] args) {
		// TODO Auto-generated method stub
		pig obj=new pig();//To access the abstract class we can done it by creating object for extended class
		obj.animalsound();
		obj.sleep(); 
	}

}
``` 
<br>

### Interface
An interface is a total abstraction class that must implement all abstract methods declared in the interface.
- By interface, we can support the functionality of multiple inheritance.
- It is used to achieve 100% abstraction.
- Every variable is by default `static` and `final`.
- Every method is by default `public` and `abstract`.
- It is used to prevent loose coupling (data leakage).
- To inherit an interface, we use the `implements` keyword, similar to the `extends` keyword.
- It is more secure than an abstract class.
- We can't create objects in an interface.

#### Example
A TV remote control is an interface, offering buttons like "power" and "volume" to interact with the TV without understanding its internal workings. You just need to know what each button does, which defines its functionality.

 ```java
interface printable{
	int age=10;//static and final
	void print();//abstract method
}

public class Interface implements printable{
	public void print() {
		System.out.println("Hello");
		
	}

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		Interface obj=new Interface();
		//age=20;//it's final by default so we can't change the value
		obj.print();
		System.out.println(printable.age);//accessing variable directly by interface name since it's static and final.
	}
}
```

<br>

### Understanding Interface Usage

Let’s say you have a class named `HDFC Bank` that has some private business logic written in the `payment` method and its object is available to use.

#### Encapsulation of Business Logic:
- HDFC Bank has a payment method that contains sensitive business logic.
- You don’t want to expose the internal implementation but still allow Amazon to use the payment functionality.
#### Why Not Use Inheritance (extends)?
- If Amazon extends HDFC Bank, it gets access to everything, including private business logic.
- This breaks encapsulation and can lead to security risks.
#### Solution: Use an Interface
- An interface declares the methods (payment in this case) without defining their implementation.
- Amazon will interact with the HDFC Bank object using the interface, ensuring controlled access.
```java
// Step 1: Define an Interface
interface PaymentGateway {
    void payment(double amount);
}

// Step 2: Implement the Interface in HDFC Bank
class HDFCBank implements PaymentGateway {
    // Private business logic inside the implementation
    @Override
    public void payment(double amount) {
        System.out.println("Processing payment of ₹" + amount + " through HDFC Bank.");
    }
}

// Step 3: Use the Interface in Amazon
class Amazon {
    private PaymentGateway paymentGateway;

    // Constructor Injection
    public Amazon(PaymentGateway paymentGateway) {
        this.paymentGateway = paymentGateway;
    }

    public void purchase(double amount) {
        System.out.println("Amazon initiating payment...");
        paymentGateway.payment(amount); // Uses HDFC Bank's payment method via interface
    }
}

// Step 4: Test the Implementation
public class Main {
    public static void main(String[] args) {
        HDFCBank hdfc = new HDFCBank(); // Object of HDFC Bank
        Amazon amazon = new Amazon(hdfc); // Amazon uses HDFC Bank via interface

        amazon.purchase(5000.0);
    }
}
```
<br>

## Encapsulation
Encapsulation is the process of binding all the data members and methods into a single entity. It ensures that the data members and methods of a class can’t be accessed directly from other classes.

### Real-World Example
Your school or office bag contains different stuff like a pen, pencil, notebook, etc. To get any stuff, you need to open the bag. Similarly, in Java, an encapsulation unit contains its data and behavior within it, and in order to access them, you need an object of that unit.


 ```java
class person {
	int mark=90; //This instance variable is openly available so anyone can access and change the value of variable 
        // leads to change of our confidential data's. Thus,it results in security issues. So to prevent this we are using private access specifier.
        // private-> it allows the data memebers,methods,constructors to be accessed only within the class
	private String name;
	private int age;
	public String getName() {
		return name;
	}
	public void setName(String name) {
		this.name=name;//why we are using this->to determine whether it's local or instance variable
	}
	public int getAge() {
		return age;
	}
	public void setAge(int age) {
		this.age=age;
	}
}
public class EncapsultaionConcept {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		person p=new person();
		p.mark=50;// instance variable value is changed by oustider. So to prevent this we are using private access specifier.
		System.out.println("Mark after variable is accessed:" +p.mark);
		p.setName("Hari");
		p.setAge(30);
		//Using Method to get the values from variables
		System.out.println("Name:"+p.getName());
		System.out.println("Age:"+p.getAge());
	}

}
```


<br>

## Polymorphism
The word ‘polymorphism’ means having many forms. In Java, polymorphism refers to the ability of a message to be displayed in more than one form.

### Real-life Example
A person can have different characteristics at the same time. Like a man at the same time is a father, a husband, and an employee. So, the same person possesses different behaviors in different situations.

```java
package EncapsulationandPolymorphism;

class human{
	public void person() {
		System.out.println("I am a person");
	}
}

class college extends human{
	public void student() {
		super.person();
		System.out.println("I am a student");
	}

}
class employee extends human{
	
	public void emp() {
		super.person();
		System.out.println("I am a employee");
	}

}
public class PolymorphismSample {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
	 employee obj=new employee();
	 obj.emp();
	 

	}

}
```
## Types of Polymorphism:

### 1.Compile-Time Polymorphism  
- Whenever an object is bound with its functionality at **compile time**, this is known as **compile-time polymorphism** (**method call is decided at compile time**).  
- Achieved through **method overloading**.  
- Also called **Early Binding**, **Static Binding**, **Static Method Dispatch**.
```java
class MathOperations {
    // Method to add two integers
    public int add(int a, int b) {
        return a + b;
    }
// Method to add three integers
    public int add(int a, int b, int c) {
        return a + b + c;
    }
    // Method to add two double values
    public double add(double a, double b) {
        return a + b;
    }
}
public class Main {
    public static void main(String[] args) {
        MathOperations mathOps = new MathOperations();
        System.out.println("Sum of 2 and 3: " + mathOps.add(2, 3));
        System.out.println("Sum of 1, 2, and 3: " + mathOps.add(1, 2, 3));
        System.out.println("Sum of 2.5 and 3.5: " + mathOps.add(2.5, 3.5));
    }
}
Explanation: In the example above, The compiler decides which method to call based on the method signature at compile time. This is why it is called Compile-Time Polymorphism.
```
  
### 2.Run-Time Polymorphism  
- Whenever an object is bound with the functionality at **run time**, this is known as **runtime polymorphism**.  
- Also known as **Dynamic Binding**, **Late Binding**, **Dynamic Method Dispatch**.  
- Achieved through **method overriding**.  

**Dynamic Method Dispatch** is the mechanism where a call to an overridden method is resolved at runtime rather than compile time.  
In this process, the overridden method that is called is based on the **actual object type**, not the reference type.  

```java
class Animal {
    void sound() {
        System.out.println("Animal makes a sound");
    }
}
class Dog extends Animal {
    @Override
    void sound() {
        System.out.println("Dog barks");
    }
}
class Cat extends Animal {
    @Override
    void sound() {
        System.out.println("Cat meows");
    }
}
public class Main {
    public static void main(String[] args) {
        Animal myAnimal = new Animal();  // Animal reference and object
        Animal myDog = new Dog();        // Animal reference but Dog object
        Animal myCat = new Cat();        // Animal reference but Cat object
        myAnimal.sound();  // Outputs: Animal makes a sound
        myDog.sound();     // Outputs: Dog barks
        myCat.sound();     // Outputs: Cat meows
    }
}
Explanation: In the example above, Animal is the superclass, and Dog and Cat are subclasses that override the sound method.The actual method that gets executed depends on the object type at runtime, which is determined by the JVM (Java Virtual Machine).

```
<br>


## **Compile-Time vs. Runtime Polymorphism**  

| Feature                     | **Compile-Time Polymorphism** | **Runtime Polymorphism** |
|-----------------------------|-----------------------------|--------------------------|
| **Other Names**             | Static Polymorphism, Early Binding| Dynamic Polymorphism, Late Binding |
| **Execution**               | method call is decided at compile time | method call is decided at run time |
| **Performance**             | **Faster** execution as it involves the compiler | **Slower** execution as it involves interpreter |
| **Inheritance**              | **Not Involved** | **Involved** |
| **Example**                 | **Method Overloading** | **Method Overriding** |


<br>

# Date and Time Functions

#### Creating Date Object
```java
//Creating Date Object
Date now = new Date();
```
<br>

#### Default Locale
```java
Locale defaultLocale = Locale.getDefault();
System.out.println(defaultLocale.getDisplayCountry());//United States
System.out.println(defaultLocale.getDisplayLanguage());//English
```
<br>

### LocalDate and LocalTime functions
```java
import java.time.LocalDate;
import java.util.Calendar;
import java.time.LocalTime;
public class LocalDateandTime {
	public  static void LocalDate() {
		LocalDate a=LocalDate.now();
		LocalDate b=LocalDate.of(2025, 10, 1); //year month 
		LocalDate c=LocalDate.parse("2024-12-12"); //(format for parse():year-month-date)
		System.out.println("Local Date: "+a);
		System.out.println("Specified date by the User using LocalDate.of(): "+b);
		System.out.println("Parsed Date:" +c);
		System.out.println("The parse date type is:"+c.getClass().getSimpleName()); // to check the type of object
	}
	public static void LocalTime() {
		LocalTime a=LocalTime.now();
		LocalTime b=LocalTime.of(2, 30, 5); //format: LocalTime.of(hr,min,sec)
		LocalTime x=LocalTime.parse("12:12:22");	
		System.out.println("Current Local Time: "+a);
		System.out.println("Specified date by the User using LocalTime.of(): "+b);
		System.out.println("Parsed time: "+x);
		System.out.println("The parse time type is: "+ x.getClass().getSimpleName());
	}
	
	
	public static void disp(){  
		LocalTime c=LocalTime.MAX;
	    LocalTime d=LocalTime.MIN;
	    LocalTime e=LocalTime.MIDNIGHT;
	    LocalTime f=LocalTime.NOON;
		System.out.println("Max time:"+c);
		System.out.println("Min time:"+d);
		System.out.println("Midnight time:"+e);
		System.out.println("Noon time:"+f);
	}
	
	public static void main(String[] args) {
		LocalDateandTime.LocalDate();
		System.out.println("---------------------------------------");
		LocalDateandTime.LocalTime();
		System.out.println("---------------------------------------");
		LocalDateandTime.disp();
		System.out.println("---------------------------------------");
		//LocalDateandTime.Calendar();
	}
}
```
<br>

#### Format Date's using SimpleDateFormat 
```java
import java.text.SimpleDateFormat;
import java.util.Date;
import java.util.Scanner;

//Question: Take Date as input from the user from a specified format and print it.
/* Steps:
 * 1.Getting User Input
 * 2.Create Object for SimpleDateFormat Class and also specify the format of the date
 * 3.Create Object for Date Class to Parse the string into date
 * 4.Printing the date using .format().
 */
public class SpecificDateFormat {
	public static void main(String[] args) {
		
		//Step 1:
		System.out.println("Enter your in dd/MM/yyyy: ");
		Scanner sc=new Scanner (System.in);
		String date_input=sc.next();
		System.out.println("The input type is: "+date_input.getClass().getSimpleName());
		
		//Step 2:
		SimpleDateFormat SDF_obj=new SimpleDateFormat("dd/MM/yyyy"); 
        //Step 3:
		try {
			Date date_obj=SDF_obj.parse(date_input); 
			System.out.println("After Parse: "+date_obj);
			System.out.println("Returning our String input as Date in Specfied Form after parse: "+SDF_obj.format(date_obj));
			System.out.println("The output type is: "+date_obj.getClass().getSimpleName());
			
		}
		catch(Exception e){
			System.out.println("Invalid Format"+ e);
		}
		sc.close();
	}
}
/* Explanation:
 * String date_input=sc.next();-> we don't know whether the user provides special characters or not so, we use next.
 *  SimpleDateFormat[under text package]->Ensures that input String is interpreted as date in specified format.
 *  MM->Month mm->Minutes
 *  parse()-> converts String into Date and returns a Date object with the value Thu Jan 01 00:00:00 IST 2025.
 *  SDF_obj.format(date_obj)->returns the Date in user specified format. (Type->Date)
 *  //If we specify 01/01/2025 instead of dd/mm/yyyy it will specify invalid format due to mismatch of date values
 */
```
<br>

### Calendar
- Calendar class is used in Java to manipulate Dates. Calendar class provides easy ways to add or reduce days, months or years from a date. It also provide lot of details about a date (which day of the year? Which week of the year? etc.)

#### Calendar is abstract
Calendar class cannot be created by using new Calendar. The best way to get an instance of Calendar class is by using getInstance() static method in Calendar. 
```java
//Calendar calendar = new Calendar(); //COMPILER ERROR
Calendar calendar = Calendar.getInstance();
```
#### Calendar set day, month and year
Setting day, month or year on a calendar object is simple. Call the set method with appropriate Constant for Day, Month or Year. Next parameter is the value.
```
calendar.set(Calendar.DATE, 24);
calendar.set(Calendar.MONTH, 8);//8 - September
calendar.set(Calendar.YEAR, 2010);
```
#### Calendar get method
Let's get information about a particular date - 24th September 2010. We use the calendar get method. The parameter passed indicates what value we would want to get from the calendar , day or month or year or .. Few examples of the values you can obtain from a calendar are listed below.
```java
System.out.println(calendar.get(Calendar.YEAR));//2010
System.out.println(calendar.get(Calendar.MONTH));//8
System.out.println(calendar.get(Calendar.DATE));//24
System.out.println(calendar.get(Calendar.WEEK_OF_MONTH));//4
System.out.println(calendar.get(Calendar.WEEK_OF_YEAR));//39
System.out.println(calendar.get(Calendar.DAY_OF_YEAR));//267
System.out.println(calendar.getFirstDayOfWeek());//1 -> Calendar.SUNDAY
```
#### Calendar - Modify a Date
We can use the calendar add and roll methods to modify a date. Calendar add method can be used to find a date 5 days or 5 months before the date by passing a ,5 i.e. a negative 5. 
```
calendar.add(Calendar.DATE, 5);
System.out.println(calendar.getTime());//Wed Sep 29 2010
calendar.add(Calendar.MONTH, 1);
System.out.println(calendar.getTime());//Fri Oct 29 2010
calendar.add(Calendar.YEAR, 2);
System.out.println(calendar.getTime());//Mon Oct 29 2012
```
<br>

# Exceptions in Java

## Exception
An exception is a wanted or unwanted event that occurs during the execution of the program at run time and disrupts the normal flow of the program. The process of handling these exceptions using `try-catch`, `throws`, and `finally` is known as Exception Handling.

## Error, Bug, and Defect
- **Error**: A mistake made by the programmer during coding.
- **Bug**: An error that is found during testing.
- **Defect**: A bug that is not caught before release.
<br>

## Types of Exceptions

### 1. User Defined Exceptions
Exceptions that are created by the user.
```java
throw new IllegalArgumentException("Age is not valid");
```
### 2. Built-in Exceptions
> #### Checked Exceptions
> > - Exceptions are checked at compile time.
> > Examples:
> > - `SQLException`
> > - `FileNotFoundException`

> #### Unchecked Exceptions
> > - Exceptions are checked at run time.
> > Examples:
> > - `NullPointerException`
> > - `ArrayIndexOutOfBoundsException`
<br>

#### Exception Handling using all Exceptions:
```java
package Exceptions;
//User defined Exception 
class InvalidAge extends Exception{
	public InvalidAge(String str) { //constructor
		super(str);   //super(str)->Calls Exception Class Constructor 
		//Exception Class Constructor accepts only String or throwbale
	}
}

public class ExceptionHandlingUsingClass {
	static void validate(int age) throws InvalidAge{ //throws class
		if(age<18){
			throw new InvalidAge("Age is not valid to vote"); //here InvalidAge is a Constructor
		}
		else {
			System.out.println("You're eligible to vote");
		}
	}
	
	public static void main(String[] args) {
		try {
			validate(14);
		}
		catch(InvalidAge e) {
			System.out.println("Caught the exception");
			System.out.println("Exception occured"+e);
		}
		System.out.println("Rest of the code");
	}
}

/*
 * If you make the constructor parameter an int and try to pass it directly to super(), 
 * it will not work because the Exception class in Java doesn't have a constructor that accepts an int. 
 * The super() call in the exception class must match one of the constructors provided by the Exception class and all of them expect either a String or a Throwable (or both).
 * Incorrect Approach (Will Cause Compilation Error):
   class RoleException extends Exception {
    public RoleException(int message) {
        super(message);  // This will cause a compilation error
    }
   }
   
   Error:
   constructor Exception in class Exception cannot be applied to given types;
   required: String
   found: int
   reason: actual argument int cannot be converted to String by method invocation conversion
```
<br>

#### Number format exception:
```java
package Exceptions;
//Integer.parseInt() -> To convert a string into particular datatype
public class NumberFormatException {

	public static void main(String[] args) {
	try {
		int num=Integer.parseInt("Hi");// this code doesn't execute Note:If a exception occured it will directly move to catch block,it wont read next line of code in try block.
                //If we use 3 it won't raise error since it is Converted to int
		int a=Integer.parseInt("3"); 
		System.out.println(num);
		System.out.println(a); 
	}
	catch(Exception e){
		System.out.println("Number Format Exception");
	}
 }

}
```
<br>

#### FileNoutFound exception:
```java
import java.io.File;
import java.io.FileReader;

//Class-> File and File Reader
public class FileNotFoundException {

	public static void main(String[] args) {
		try {
			File f=new File("C:\\Users\\harih\\OneDrive\\Documents\\Java\\JavaProgramming\\src\\Exceptions\\ExceptionHandling.java");
			FileReader fr=new FileReader(f);
			System.out.println("File Exists");
		}
		catch(Exception e) { //FileNotFoundException
			System.out.println("File Does Not Exist");
		}
	}
}

```
<br>

#### OneTryManyCatch:
```java
public class OneTryManyCatch {
	public static void main(String[] args) {
	try {
		int a[]=new int[5];
		System.out.println(a[4]);
	}
	
	catch(ArithmeticException e) {
		System.out.println("Arithmetic Exception Occurs");
	}
	catch(ArrayIndexOutOfBoundsException e) {
		System.out.println("Array Index Out Of Bound Exception Occurs");
	}
	catch(Exception e) {
		System.out.println("Parent Exception Occurs");
	}
	System.out.println("Rest of Code");
	}

}
```
<br>

### `throw` vs `throws`

| Feature  | `throw` | `throws` |
|----------|--------|---------|
| **Definition** | Used to explicitly throw an exception inside a function or block of code. | Used in the method signature to indicate whether an exception may occur or not. |
| **Location** | Used inside a method or block of code. | Used in the method signature (main) and also in normal methods. |
| **Usage** | Can throw both checked and unchecked exceptions. | Only used for checked exceptions. Unchecked exceptions do not require `throws`. |
| **Internal Implementation** | Only one exception can be thrown at a time. | Multiple exceptions can be declared using `throws`. |
| **Example** | `throw new ArithmeticException("Error");` | `public void myMethod() throws IOException {}` |
<br>

### Final Keyword
The `final` keyword is a non-access modifier used to indicate that a variable, method, or class cannot be modified after it is initialized or defined.

### Uses of `final`
- **Final Variables**: Once a variable is declared as `final`, its value cannot be changed.
- **Final Methods**: A method declared as `final` cannot be overridden by subclasses. *(Final methods can be overloaded.)*
- **Final Classes**: A class declared as `final` cannot be extended by other classes.
<br>

### `finally` Keyword
A `finally` block is used to execute a particular process regardless of whether an exception is thrown or not and ensures that cleanup code runs.
- The `finally` block is always executed after the `try` and `catch` blocks.
- **Note**: The `finally` block is always executed unless there is an unhandled exception that terminates the program.
- **Will `finally` block return a value?** No, it will not return any value.
<br>

### `finalize` Method
The `finalize()` method in Java is a method of the `Object` class, called by the Garbage Collector to perform cleanup activities before destroying an object from memory.

#### Syntax
```java
protected void finalize() throws Throwable {
    // Cleanup code
}
```
#### Why Use `finalize()`?
Before the Garbage Collector deletes an object, the `finalize()` method releases all resources the object uses. Once `finalize()` executes, the Garbage Collector immediately eliminates the Java object.
<br>

# Arrays
Array are used to store multiple values in a single variable instead of declaring separate variables for each values

### How to access the element for an array?
 - we can access the array element by index no changing an array element 
 - To change the value of the specific elements refer to the index number
 - **array length** -> to find how many elements an array has,use the length property
 -If we access an array out of the array size which is not specified(since array size is finished) 
 -It will raise out-of-index error and returns -1 due to backward indexing

### What is traverse an array?
   > You can traverse through an array using for loop or enhanced-for which means you can iterate the index using 
   > loop starting from 0 to length of the array and access element at each index

 **Arrays.fill** -> This method assigns the specified data-type value to each element of the specified range of the specified array
 
```java
 How to initialize array value?
 Type 1-> If we want to store element values in an array use new keyword
 int[] arr= new int[]{1,2,3} // used in corporates
 Type 2-> Java allows short-hand declaration for array initialization
 int[] arr={0,9} (if we declare size in int it will use only that size only)
 Type 3-> No change in functionality but not on size
 int arr[]={98,99}
 Type 4->initializes the array value
 int arr[]=new int[4]
```
```java
//Declaring an Array
int[] marks;

// Creating an array
marks = new int[5]; // 5 is size of array

int marks2[] = new int[5];//Declaring and creating an array in same line.

System.out.println(marks2[0]);//New Arrays are always initialized with default values - 0

//Index of elements in an array runs from 0 to length - 1
marks[0] = 25;
marks[1] = 30;
marks[2] = 50;
marks[3] = 10;
marks[4] = 5;

System.out.println(marks[2]);//Printing a value from array

//Printing a 1D Array
int marks5[] = { 25, 30, 50, 10, 5 };
System.out.println(marks5); //[I@6db3f829
System.out.println(
    Arrays.toString(marks5));//[25, 30, 50, 10, 5]

int length = marks.length;//Length of an array: Property length

//Enhanced For Loop
for (int mark: marks) {
    System.out.println(mark);
}

//Fill array with a value
Arrays.fill(marks, 100); //All array values will be 100

//String Arrays
String[] daysOfWeek = { "Sunday", "Monday", "Tuesday", "Wednesday", "Thursday", "Friday", "Saturday" };
```

### 2D Arrays

Best way to visualize a 2D array is as an array of arrays.

```java
int[][] matrix = { { 1, 2, 3 }, { 4, 5, 6 } };

int[][] matrixA = new int[5][6]; 

//Accessing elements from 2D array:
System.out.println(matrix[0][0]); //1
System.out.println(matrix[1][2]); //6

//Looping a 2D array
for (int[] array: matrix) {
    for (int number: array) {
         System.out.println(number);
    }
}

// Printing a 2D Array
int[][] matrix3 = { { 1, 2, 3 }, { 4, 5, 6 } };
System.out.println(matrix3); //[[I@1d5a0305
System.out.println(

Arrays.toString(matrix3)); 
//[[I@6db3f829, [I@42698403]

System.out.println(Arrays.deepToString(matrix3)); 
//[[1, 2, 3], [4, 5, 6]]

System.out.println(matrix3[0]);//[I@86c347 - matrix3[0] is a 1D Array
System.out.println(Arrays.toString(matrix3[0]));//[1, 2, 3]
```

### Other Array Operations

```java
//Comparing Arrays
int[] numbers1 = { 1, 2, 3 };
int[] numbers2 = { 4, 5, 6 };

System.out.println(Arrays
.equals(numbers1, numbers2)); //false

int[] numbers3 = { 1, 2, 3 };

System.out.println(Arrays
.equals(numbers1, numbers3)); //true

// Sorting an Array

int rollNos[] = { 12, 5, 7, 9 };
Arrays.sort(rollNos);
System.out.println(Arrays.toString(rollNos));//[5, 7, 9, 12]

```

### Array of Objects
**Array of objects:** Creating array for  objects.
- Array of objects is used to store multiple instances of class within single array. This allows us to easy manage a collections of objects.

```java
Person[] persons = new Person[3];

//By default, an array of 3 reference variables is created.

//The person objects are not created
System.out.println(persons[0]);//null

//Let's create the new objects
persons[0] = new Person();
persons[1] = new Person();
persons[2] = new Person();

//Creating and initializing person array in one statement
Person[] personsAgain = { new Person(),new Person(),new Person()};

//Another example
Person[][] persons2D = 
    {
		{ new Person(),new Person(),new Person()},
		{ new Person(),new Person()}
    };
```
<br>

### Class of Objects
 **Class of Objects:** Creating array for class.
```java
class Student{
	public String name;
	public int id;
	Student(int id,String name){
		this.id=id;
		this.name=name;
		
	}
	public void display() {
		System.out.println("Student Id & name is "+id+" "+name);
	}
	 public String toString() {
	        return "id=" + id + ", name='" + name + "'";
	    }
	
}
public class ClassofObjects {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		Student[] arr= new Student[10];
		arr[0]=new Student(100,"hari");
		arr[1]=new Student(100,"dk");
		arr[2]=new Student(200,"kumar");
		arr[3]=new Student(300,"saran");
		arr[0].display();
		arr[1].display();
		System.out.println("Another Way of passing Array Elements: ");
		Student[] arr1= { new Student(16,"Hari"),new Student(11,"DK"),new Student(29,"Kumaravel")};
		System.out.println(Arrays.toString(arr1));
	}
}
```
<br>

#### Array Tips 
```java

//You can Declare, Create and Initialize Array on same line.
int marks3[] = { 25, 30, 50, 10, 5 };

//Leaving additional comma is not a problem. (note that comma after 5)
int marks4[] = { 25, 30, 50, 10, 5, };


int marks[]; //Not Readable
int[] runs; //Readable


//int values[5];//Compilation Error!Declaration of an Array should not include size. 

//marks = new int[];//COMPILER ERROR! Size of an array is mandatory to create an array.


//Declaring 2D Array Examples:
int[][] matrix1; //Recommended
int[] matrix2[]; //Legal but not readable. Avoid.

//Access 10th element when array has only length 5
//Runtime Exception: ArrayIndexOutOfBoundsException
//System.out.println(marks[10]);

//Array can contain only values of same type.

//COMPILE ERROR!!
//int marks4[] = {10,15.0}; //10 is int 15.0 is float

//Cross assigment of primitive arrays is ILLEGAL
int[] ints = new int[5];
short[] shorts = new short[5];
//ints = shorts;//COMPILER ERROR
//ints = (int[])shorts;//COMPILER ERROR


//The first dimension of a 2D array is mandatory
matrixA = new int[3][];//FINE
//matrixA = new int[][5];//COMPILER ERROR
//matrixA = new int[][];//COMPILER ERROR

//Each row in a 2D Array can have a different size. This is called a Ragged Array.
matrixA = new int[3][];//FINE
matrixA[0] = new int[3];
matrixA[0] = new int[4];
matrixA[0] = new int[5];
```

# String Class

- A String class can store a sequence of characters. String is not a primitive in Java but a Class in its own right. String can be a letter,number,symbol,spaces.

## Strings are immutable

- Value of a String Object once created cannot be modified. Any modification on a String object creates a new String object.

```java
String str3 = "value1";
str3.concat("value2");
System.out.println(str3); //value1
```

Note that the value of str3 is not modified in the above example.  The result should be assigned to a new reference variable (or same variable can be reused).

```java
String concat = str3.concat("value2");
System.out.println(concat); //value1value2
```


## String vs StringBuffer vs StringBuilder
- Immutability : String
- Thread Safety : String(immutable), StringBuffer
- Performance : StringBuilder (especially when a number of modifications are made.)
- [Example 1](src/main/java/com/in28minutes/java/string/StringBufferBuilderExamples.java)


#### String Constant Pool
- The string pool, also known as the string constant pool, is a special storage area in the Java heap memory where the JVM stores string literals.
- All strings literals are stored in "String constant pool". If compiler finds a String literal,it checks if it exists in the pool. If it exists, it is reused.

- Following statement creates 1 string object (created on the pool) and 1 reference variable.

```java
String str1 = "value"; 
```

- However, if new operator is used to create string object, the new object is created on the heap. Following piece of code create 2 objects.

```java
//1. String Literal "value" - created in the "String constant pool"
//2. String Object - created on the heap
String str2 = new String("value");
```
![image](https://github.com/user-attachments/assets/778ae5dc-008d-4e18-a10c-96deedad6fce)

#### String Method Examples

String class defines a number of methods to get information about the string content.

```java
String str = "abcdefghijk";
```

##### Get information from String

Following methods help to get information from a String.

```java
//char charAt(int paramInt)
System.out.println(str.charAt(2)); //prints a char - c
System.out.println("ABCDEFGH".length());//8
System.out.println("abcdefghij".toString()); //abcdefghij
System.out.println("ABC".equalsIgnoreCase("abc"));//true

//Get All characters from index paramInt
//String substring(int paramInt)
System.out.println("abcdefghij".substring(3)); //defghij

//All characters from index 3 to 6
System.out.println("abcdefghij".substring(3,7)); //defg

String s1 = new String("HELLO"); 
String s2 = new String("HELLO"); 
System.out.println(s1 == s2); // false
System.out.println(s1.equals(s2)); // true
```

#### String Manipulation methods

Most important thing to remember is a String object cannot be modified. When any of these methods are called, they return a new String with the modified value. The original String remains unchanged.

```java
//String concat(String paramString)
System.out.println(str.concat("lmn"));//abcdefghijklmn

//String replace(char paramChar1, char paramChar2)
System.out.println("012301230123".replace('0', '4'));//412341234123

//String replace(CharSequence paramCharSequence1, CharSequence paramCharSequence2)
System.out.println("012301230123".replace("01", "45"));//452345234523

System.out.println("ABCDEFGHIJ".toLowerCase()); //abcdefghij

System.out.println("abcdefghij".toUpperCase()); //ABCDEFGHIJ

//trim removes leading and trailings spaces
System.out.println(" abcd  ".trim()); //abcd
```
### String Concatenation Operator

#### Three Rules of String Concatenation
- RULE1: Expressions are evaluated from left to right. Except if there are parenthesis.
- RULE2: number + number = number
- RULE3: number + String = String

```java
System.out.println(5 + "Test" + 5); //5Test5
System.out.println(5 + 5 + "Test"); //10Test
System.out.println("5" + 5 + "Test"); //55Test
System.out.println("5" + "5" + "25"); //5525
System.out.println(5 + 5 + "25"); //1025
System.out.println("" + 5 + 5 + "25"); //5525
System.out.println(5 + (5 + "25")); //5525
System.out.println(5 + 5 + 25); //35
```
<br>

#### String Buffer Examples
```java
StringBuffer stringbuffer = new StringBuffer("12345");
stringbuffer.append("6789");
System.out.println(stringbuffer); //123456789
//All StringBuffer methods modify the value of the object.
```
#### String Builder Examples
```java
StringBuilder sb = new StringBuilder("0123456789");

//StringBuilder delete(int startIndex, int endIndexPlusOne)
System.out.println(sb.delete(3, 7));//012789

StringBuilder sb1 = new StringBuilder("abcdefgh");

//StringBuilder insert(int indext, String whatToInsert)
System.out.println(sb1.insert(3, "ABCD"));//abcABCDdefgh

StringBuilder sb2 = new StringBuilder("abcdefgh");
//StringBuilder reverse()
System.out.println(sb2.reverse());//hgfedcba
```
Similar functions exist in StringBuffer also.
<br>

# Collections Framework

## What is Collection?
- Collection refers to a group of objects represented as single unit.

## What are Collection Frameworks?
- Collection Frameworks are sets of classes and interfaces that provide a ready-made architecture for storing and manipulating groups of objects(data) as a single unit.
- It contains interfaces, classes, iterators to implement various Data Structures and Algorithms.

## Why Collection Framework?

## What are the main interfaces in the Collection Framework?
The core interfaces are:
- `Collection`: The root interface representing a group of objects.
- `List`: An ordered collection (sequence) that allows duplicate elements.
- `Set`: A collection that does not allow duplicate elements.
- `Queue`: A collection used to hold multiple elements prior to processing.
- `Map`: An object that maps keys to values.
<br>

