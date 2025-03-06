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

