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

[Watch this video](https://youtu.be/7yr81Dnn0NY?si=a5Yc6NEeBfCkoqlT) for more details.

![zp](https://github.com/user-attachments/assets/f30c99df-1027-47b1-8beb-2f93aa558c51)


## Java Architecture:

![image](https://github.com/user-attachments/assets/3a28630b-7162-4102-846f-110b0507cee6)

# Java Development Environment

## 1. JDK (Java Development Kit)
The Java Development Kit (JDK) provides the necessary environment to develop and execute Java programs. It includes essential tools such as:
- Compiler
- Archiver
- Debugger
- Java Runtime Environment (JRE)
- Other development tools

JDK is platform-dependent, meaning separate installers are required for Windows, Unix, and Mac operating systems.

### JDK Components:
- **Development Tools**: Provides an environment to develop Java programs.
- **JRE (Java Runtime Environment)**: Allows execution of Java programs.

## 2. JRE (Java Runtime Environment)
The Java Runtime Environment (JRE) is a software package that provides an environment to run (but not develop) Java programs on a machine. It contains:
- **JVM (Java Virtual Machine)**
- **Libraries**
- **Other essential components**

JRE is primarily used for running Java applications and does not include development tools.

## 3. JVM (Java Virtual Machine)
The Java Virtual Machine (JVM) is a virtual CPU that provides a runtime environment for executing Java bytecode. It is responsible for:
- Converting bytecode into machine-specific code.
- Loading class files using the class loader.
- Verifying bytecode integrity with the bytecode verifier.
- Executing bytecode line by line, functioning as an interpreter.

## 4. JIT (Just-In-Time Compiler)
The Just-In-Time (JIT) Compiler is a component of the JVM that enhances Java application performance by compiling bytecodes into native machine code at runtime.






