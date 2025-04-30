📘 Full Detailed Notes: Java 8 Basics for CDAC CCPP
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

java
Copy
Edit
import java.util.Scanner;
➡ c) Difference between Object Reference Variables and Primitive Variables

Type	Example	Stored
Primitive Variable	int x = 10;	Stores actual value.
Reference Variable	String s = "hello";	Stores memory address (reference) of object.
➡ d) How to Read and Write to Object Fields
Access fields using . operator.

🔹 Example:

java
Copy
Edit
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
📌 1. Who is known as the father of Java programming language?
a) Dennis Ritchie
b) James Gosling
c) Bjarne Stroustrup
d) Guido van Rossum

Answer: b) James Gosling

📌 2. Which feature of Java is responsible for "Write Once, Run Anywhere"?
a) Object-Oriented
b) Platform Dependent
c) Bytecode
d) Dynamic

Answer: c) Bytecode

📌 3. Java programs are compiled into ________.
a) Assembly code
b) Machine code
c) Bytecode
d) Source code

Answer: c) Bytecode

📌 4. What is the output of the Java compiler (javac)?
a) .java file
b) .exe file
c) .class file
d) .html file

Answer: c) .class file

📌 5. Which of the following is NOT a Java feature?
a) Platform Independent
b) Secure
c) Architecture Neutral
d) Pointer Arithmetic

Answer: d) Pointer Arithmetic

📌 6. Which type of variable is declared inside a method?
a) Static variable
b) Instance variable
c) Local variable
d) Global variable

Answer: c) Local variable

📌 7. Which keyword is used to inherit a class in Java?
a) extends
b) inherits
c) implements
d) super

Answer: a) extends

📌 8. In Java, polymorphism refers to:
a) Many methods with same name but different signatures
b) Many classes with the same parent
c) Many variables with same value
d) Many loops inside a method

Answer: a) Many methods with same name but different signatures

📌 9. Which of these is not a primitive data type in Java?
a) int
b) boolean
c) float
d) String

Answer: d) String

📌 10. Which memory area stores objects in Java?
a) Stack
b) Heap
c) PC Register
d) Native Stack

Answer: b) Heap

📌 11. Which tool is used to create documentation from Java source code comments?
a) javac
b) javadoc
c) java
d) jdb

Answer: b) javadoc

📌 12. Which part of JVM executes Java bytecode?
a) Compiler
b) Execution Engine
c) Class Loader
d) Garbage Collector

Answer: b) Execution Engine

📌 13. Which package is automatically imported in every Java program?
a) java.util
b) java.io
c) java.lang
d) java.awt

Answer: c) java.lang

📌 14. What happens when an object is no longer referenced?
a) JVM compiles it again
b) Garbage Collector deletes it
c) It stays forever in memory
d) It throws exception

Answer: b) Garbage Collector deletes it

📌 15. Which keyword is used to define a constant variable in Java?
a) final
b) static
c) const
d) constant

Answer: a) final

📌 16. What is the extension of a Java compiled file?
a) .java
b) .exe
c) .class
d) .txt

Answer: c) .class

📌 17. Which memory area stores method parameters and local variables?
a) Heap
b) Stack
c) Method Area
d) Native Stack

Answer: b) Stack

📌 18. How many times is the static variable initialized?
a) Every time an object is created
b) Only once when the class is loaded
c) Each time method is called
d) None of the above

Answer: b) Only once when the class is loaded

📌 19. The "main" method in Java must be:
a) Private and static
b) Public and static
c) Protected and static
d) Private and abstract

Answer: b) Public and static

📌 20. Which of the following is responsible for loading classes in JVM?
a) Execution Engine
b) Class Loader
c) Memory Manager
d) JDK

Answer: b) Class Loade
_________________________________________________________________________________________________________________________
:

📚 1. Instance Variable
Declared inside a class, but outside any method.

Belongs to an object — each object has its own copy.

Value can be different for different objects.

Created when object is created and destroyed when object is destroyed.

✅ Example:

java
Copy
Edit
class Student {
    int rollNumber;  // Instance Variable
    String name;     // Instance Variable

    void display() {
        System.out.println(rollNumber + " " + name);
    }
}

public class Test {
    public static void main(String[] args) {
        Student s1 = new Student();
        s1.rollNumber = 101;
        s1.name = "John";

        Student s2 = new Student();
        s2.rollNumber = 102;
        s2.name = "Alice";

        s1.display();
        s2.display();
    }
}
🔵 Output:

Copy
Edit
101 John
102 Alice
📚 2. Static Variable
Declared using the static keyword inside a class.

Belongs to the class, not to objects.

Shared among all objects — only one copy exists.

Can be accessed using class name also.

✅ Example:

java
Copy
Edit
class Student {
    int rollNumber;
    String name;
    static String college = "ABC College";  // Static Variable

    void display() {
        System.out.println(rollNumber + " " + name + " " + college);
    }
}

public class Test {
    public static void main(String[] args) {
        Student s1 = new Student();
        s1.rollNumber = 101;
        s1.name = "John";

        Student s2 = new Student();
        s2.rollNumber = 102;
        s2.name = "Alice";

        s1.display();
        s2.display();
    }
}
🔵 Output:

Copy
Edit
101 John ABC College
102 Alice ABC College
📚 3. Local Variable
Declared inside a method, constructor, or block.

Scope is only within that method — not visible outside.

Must be initialized before use.

Memory allocated only when method is called, and destroyed after method ends.

✅ Example:

java
Copy
Edit
class Test {
    void show() {
        int num = 10; // Local Variable
        System.out.println(num);
    }

    public static void main(String[] args) {
        Test t = new Test();
        t.show();
    }
}
🔵 Output:

Copy
Edit
10
⚡ Important Point:
Local variables do not get default values — you have to manually initialize them!

📑 Quick Summary Table:

Type of Variable	Where Declared	Lifetime	Scope	Shared?
Instance Variable	Inside class, outside methods	Till object exists	Throughout object	No
Static Variable	Inside class with static keyword	Till program ends	Throughout class	Yes (common for all objects)
Local Variable	Inside methods, blocks, constructors	During method execution	Inside method only	No
