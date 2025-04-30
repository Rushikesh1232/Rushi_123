1. Overview of Java
Java is a general-purpose, high-level, class-based, object-oriented programming language.

Developed by James Gosling at Sun Microsystems in 1995.

Java programs are compiled into bytecode, which runs on the Java Virtual Machine (JVM) — making Java platform-independent.

🔹 Java Motto: "Write Once, Run Anywhere (WORA)"

Main Areas where Java is used:

Desktop GUI Applications (Swing, JavaFX)

Web-based applications (JSP, Servlet)

Mobile apps (Android)

Distributed applications

Cloud-based services

Game development

2. Features of Java

Feature	Description
Simple	Easy to learn; syntax is simple compared to C++ (no pointers).
Object-Oriented	Everything is an object (except primitive data types).
Platform Independent	Bytecode runs on any system with JVM.
Secured	Prevents unauthorized access, virus-free.
Robust	Strong memory management, exception handling.
Multithreaded	Can perform multiple tasks simultaneously.
Distributed	Supports distributed computing using RMI, EJB.
High Performance	Bytecode execution + Just In Time (JIT) compiler increases speed.
Portable	No dependency on architecture (CPU, OS).
Dynamic	Supports dynamic loading of classes at runtime.
3. Scope of Variables in Java

Type	Description	Lifetime
Local Variables	Declared inside method or block.	Exist until method finishes.
Instance Variables	Declared inside a class, but outside any method.	Exist until object is alive.
Static Variables	Declared with static keyword inside class. Shared among all objects.	Exist for the lifetime of class in memory.
🔹 Example:

java
Copy
Edit
class Example {
    static int staticVar = 100;   // static variable
    int instanceVar = 50;         // instance variable

    void method() {
        int localVar = 10;        // local variable
        System.out.println(localVar);
    }
}
4. Object-Oriented Concepts (OOPS)
➡ 4 Main Pillars:

Pillar	Meaning
Encapsulation	Wrapping data (fields) and methods into a single unit (class).
Inheritance	One class inherits properties of another (extends keyword).
Polymorphism	Same method behaves differently (overloading/overriding).
Abstraction	Hiding internal details; showing only functionality (abstract class, interface).
🔹 Example:

java
Copy
Edit
class Animal {
    void sound() {
        System.out.println("Animal makes a sound");
    }
}

class Dog extends Animal {
    void sound() {
        System.out.println("Dog barks");
    }
}
5. Java Virtual Machine (JVM) Overview
JVM is an abstract machine that enables your Java program to run.

It converts bytecode (.class file) into machine-specific code.

It provides:

Memory Management (Heap, Stack)

Garbage Collection (automatic memory cleaning)

Security and Exception Handling

Execution of programs

🔹 JVM Architecture:


Component	Description
Class Loader	Loads class files.
Runtime Data Areas	Method Area, Heap, Java Stack, PC Register, Native Method Stack.
Execution Engine	Executes bytecode instructions.
Garbage Collector	Frees up memory.
6. JDK and its Usage

Term	Full Form	Purpose
JDK	Java Development Kit	Complete development kit (compiler + JRE + tools).
JRE	Java Runtime Environment	Provides environment to run Java applications.
JVM	Java Virtual Machine	Part of JRE, runs compiled bytecode.
🔹 Important Java Tools in JDK:


Tool	Function
javac	Java Compiler: Compiles .java into .class.
java	Java Interpreter: Runs .class files.
jdb	Java Debugger: Debugging tool for Java programs.
javadoc	Documentation generator from Java source code comments.
🔹 Example:

bash
Copy
Edit
javac HelloWorld.java    # Compile source code
java HelloWorld          # Run compiled class
7. Working with Data Types
➡ a) Structure of a Java Class
Basic structure:

java
Copy
Edit
import java.util.Scanner; // importing package

public class MyClass {
    int number; // instance variable

    public void display() {
        System.out.println("Number: " + number);
    }

    public static void main(String[] args) {
        MyClass obj = new MyClass();
        obj.number = 10;
        obj.display();
    }
}
➡ b) Importing Packages
Packages are like folders containing classes.

To use classes from another package, use import.

🔹 Example:
import java.util.Scanner;
➡ c) Difference between Object Reference Variables and Primitive Variables

Type	Example	Stored
Primitive Variable	int x = 10;	Stores actual value.
Reference Variable	String s = "hello";	Stores memory address (reference) of object.
➡ d) How to Read and Write to Object Fields
Access fields using . operator.

🔹 Example:
class Student {
    int id;
    String name;
}

class Main {
    public static void main(String[] args) {
        Student s1 = new Student();
        s1.id = 101;      // writing
        s1.name = "John"; // writing

        System.out.println(s1.id);   // reading
        System.out.println(s1.name); // reading
    }
}
📚 Summary Table of All Topics

Topic	Key Points
Overview of Java	Platform-independent, compiled to bytecode.
Features	Simple, Object-Oriented, Secure, Portable, Robust, etc.
Scope of Variables	Local, Instance, Static.
OOPS Concepts	Encapsulation, Inheritance, Polymorphism, Abstraction.
JVM	Converts bytecode into machine code, manages memory.
JDK Tools	Compiler (javac), Interpreter (java), Debugger (jdb), Documentation (javadoc).
Data Types	Primitive (int, boolean) vs Object (String, Scanner).
Accessing Object Fields	Using dot (.) operator.
📝 MCQs for Practice - CDAC CCPP Level
Q1: Who invented Java?
a) Dennis Ritchie
b) James Gosling
c) Charles Babbage
d) Guido van Rossum
Answer: b) James Gosling

Q2: Which feature of Java allows it to be platform-independent?
a) Compilation
b) Bytecode
c) Object-Oriented
d) Exception Handling
Answer: b) Bytecode

Q3: What is the default value of a local variable in Java?
a) 0
b) null
c) Depends on type
d) No default value
Answer: d) No default value

Q4: What is the purpose of the javac command?
a) To interpret code
b) To debug code
c) To compile code
d) To run code
Answer: c) To compile code

Q5: Which of the following is NOT a primitive data type?
a) int
b) float
c) boolean
d) String
Answer: d) String

Q6: In Java, "Encapsulation" is achieved by?
a) Inheritance
b) Interfaces
c) Classes and Access Modifiers
d) Abstract Classes
Answer: c) Classes and Access Modifiers

Q7: What does JVM stand for?
a) Java Verified Machine
b) Java Visual Machine
c) Java Virtual Machine
d) Java Variable Method
Answer: c) Java Virtual Machine

Q8: In Java, which keyword is used to inherit a class?
a) implement
b) inherit
c) extends
d) this
Answer: c) extends
