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


