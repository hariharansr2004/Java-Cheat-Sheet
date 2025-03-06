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
<br>

### Scanner Class
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

** Nested switch:**
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
### toString() Method
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

##  Instance Variable vs. Static Variable vs. Local Variable

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
Call by Value Explanation in detail:

**NOTE: Java doesn't have CallByReference because java doesn't support pointers.**

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
| Invocation        | Called only once at the time of object creation | Can be called any number of times |
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
- As per java rule whenever we create object for subclass object its super class constructor must be called in-order to complete the constructor chaining process.
- But in Multiple inheritance one subclass will have more than one superclass, when we create object of the subclass the JVM will get confuse which superclass constructor it should execute first to complete the constructor chaining.
- To avoid this confusion multiple inheritance is not allowed in java.
  
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
<br>

## Important Points About this() and super() in Java
- this() as well super() can be used exactly once inside the constructor.
- If we use this() followed by super() or super() followed by this() we will get compile-time error. It is due to either this() or super() can be the first statement inside the constructor, not both.
Inside the constructor, we cannot call the this() and super() recursively. 
<br>

## Interview Question: When Do You Need a `super` Keyword?

- Whenever a derived class inherits the features of a base class, there is a chance that base class features are similar to derived class features, resulting in ambiguity for the JVM. The `super` keyword must be used to distinguish between base class features and derived class features.

## Can We Use Both `this()` and `super()` in the Same Constructor?

- No, Both this() and super() cannot be used together in constructor.
- this() is used to call default constructor of same class.it should be first statement inside constructor.
- super() is used to call default constructor of base class.it should be first statement inside constructor.
- so this() and super() both are used for constructor call but both want to execute at first. that's why it'll show compiler error like :
```java
error: call to this must be first statement in constructor this(); or

error: call to this must be first statement in constructor super();
```

<br>


