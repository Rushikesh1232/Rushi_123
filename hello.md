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
_________________________________________________________________________________________________________________________
 1. JVM (Java Virtual Machine)
✅ What is JVM?
JVM stands for Java Virtual Machine.

It is an abstract machine that enables your computer to run Java programs.

JVM is platform-dependent, but Java code is platform-independent because of the JVM.

🔧 Responsibilities of JVM:
Loads the .class file (compiled bytecode).

Verifies the bytecode to ensure security.

Interprets or compiles the bytecode to native machine code.

Manages memory (via Garbage Collection).

Handles exceptions and ensures security.

🔁 How it works:
java
Copy
Edit
// You write a Java program
public class Hello {
   public static void main(String[] args) {
      System.out.println("Hello CDAC!");
   }
}
javac Hello.java → Compiled to Hello.class (Bytecode)

java Hello → JVM runs the bytecode in Hello.class

📌 Note:
JVM is the reason Java is "Write Once, Run Anywhere".

🔹 2. JRE (Java Runtime Environment)
✅ What is JRE?
JRE = JVM + Libraries + Other Files

It is the runtime environment required to run Java programs.

It does not include development tools like compilers or debuggers.

🧩 JRE Contains:
JVM

Java Class Libraries (e.g., java.lang, java.util)

Supporting files (like configuration files)

📌 Note:
If you only want to run Java programs, install JRE.

Example: End-users who use Java-based apps.

🔹 3. JDK (Java Development Kit)
✅ What is JDK?
JDK = JRE + Development Tools

It is a full package for Java developers.

🧰 JDK Contains:
JRE (JVM + Libraries)

javac (Java Compiler)

javadoc (Documentation generator)

jar (Packaging tool)

debuggers and other development tools

📌 Note:
If you want to write, compile, and run Java programs, install JDK.

🔹 4. JIT (Just-In-Time Compiler)
✅ What is JIT?
JIT is part of the JVM.

It improves performance by compiling bytecode into native machine code at runtime.

🔧 How it works:
Initially, JVM interprets bytecode line by line.

When it detects frequently used code (hotspot), it compiles it to native code.

Native code is faster, improving performance.

📌 Types of JIT:
Method-level JIT: Compiles entire methods.

Adaptive JIT: Learns and optimizes over time.

🧠 Summary Table
Component	Stands For	Contains	Purpose
JVM	Java Virtual Machine	—	Runs bytecode
JRE	Java Runtime Environment	JVM + Libraries	Runs Java applications
JDK	Java Development Kit	JRE + Tools	Develops and runs Java apps
JIT	Just-In-Time Compiler	Part of JVM	Boosts performance by compiling at runtime

___________________________________________________________________________________________________________________________________________________________


 A. Primitive Data Types (8 Types)
1. byte – 1 Byte (8 bits)
Smallest integer data type.

Range: -128 to 127

java
Copy
Edit
byte a = 10;
System.out.println("Byte value: " + a);
2. short – 2 Bytes (16 bits)
Larger than byte but smaller than int.

Range: -32,768 to 32,767

java
Copy
Edit
short s = 20;
System.out.println("Short value: " + s);
3. int – 4 Bytes (32 bits)
Most commonly used integer type.

Range: -2^31 to 2^31-1

java
Copy
Edit
int i = 30;
System.out.println("Int value: " + i);
4. long – 8 Bytes (64 bits)
Used when int is not large enough.

Add L at the end of the value

java
Copy
Edit
long l = 40L;
System.out.println("Long value: " + l);
5. float – 4 Bytes (32 bits)
Used for decimal numbers.

Add f at the end of the value

java
Copy
Edit
float f = 3.14f;
System.out.println("Float value: " + f);
6. double – 8 Bytes (64 bits)
More precise than float, default for decimals

java
Copy
Edit
double d = 9.8;
System.out.println("Double value: " + d);
7. char – 2 Bytes (16 bits)
Stores a single character in single quotes

java
Copy
Edit
char c = 'A';
System.out.println("Char value: " + c);
8. boolean – 1 Byte (usually 1 bit)
Stores only true or false

java
Copy
Edit
boolean b = true;
System.out.println("Boolean value: " + b);
__________________________________________________________________________________________________________________________________________________________
All data type exampls 

public class DataTypesExample {
    public static void main(String[] args) {
        byte a = 10;
        short s = 20;
        int i = 30;
        long l = 40L;
        float f = 3.14f;
        double d = 9.8;
        char c = 'A';
        boolean b = true;

        System.out.println("Byte value: " + a);
        System.out.println("Short value: " + s);
        System.out.println("Int value: " + i);
        System.out.println("Long value: " + l);
        System.out.println("Float value: " + f);
        System.out.println("Double value: " + d);
        System.out.println("Char value: " + c);
        System.out.println("Boolean value: " + b);
    }
}

__________________________________________________________________________________________________________________________________________________________


 8. Type Casting in Java
Type Casting means converting a variable from one data type to another. In Java, this is mainly of two types:

🔹 A. Widening Casting (Implicit)
➡️ Converting a smaller type to a larger type size
➡️ Done automatically by Java – no data loss

✅ Types Order (Small to Big):
arduino
Copy
Edit
byte → short → int → long → float → double
🧠 Example:
java
Copy
Edit
int a = 10;        // int is 4 bytes
long b = a;        // long is 8 bytes - bigger than int
System.out.println("Widening: " + b);
✅ Output:
makefile
Copy
Edit
Widening: 10
📌 Why allowed?
No loss of data

JVM handles it automatically

🔹 B. Narrowing Casting (Explicit)
➡️ Converting a larger type to a smaller type size
➡️ You must explicitly cast using (type)
➡️ Possible data loss

🧠 Example:
java
Copy
Edit
double d = 9.5;       // double is 8 bytes
int i = (int) d;      // Explicit cast: double → int
System.out.println("Narrowing: " + i);
✅ Output:
makefile
Copy
Edit
Narrowing: 9
⚠️ What happened?
Decimal part .5 is truncated

Only the whole number is stored

📊 Summary Table
Type Casting	Direction	Example Code	Safe?	Automatic?
Widening	Small → Big	int a = 10; long b = a;	✅ Safe	✅ Yes
Narrowing	Big → Small	double d = 9.5; int i = (int)d;	⚠️ Data loss	❌ No
__________________________________________________________________________________________________________________________📚 Object's Lifecycle in Java
In Java, an Object goes through three main stages:

Creation

Reassignment

Garbage Collection
(including finalize() method)

1. 📌 Object Creation
In Java, objects are created using the new keyword.

When you use new, Java:

Allocates memory in Heap.

Calls the constructor to initialize the object.

✅ Example:

java
Copy
Edit
class Student {
    Student() {
        System.out.println("Student object created");
    }
}

public class Test {
    public static void main(String[] args) {
        Student s = new Student();  // Object creation
    }
}
🔵 Output:

csharp
Copy
Edit
Student object created
⚡ Key Point:
Memory is assigned in Heap Memory when new is used.

2. 📌 Object Reassignment
Reassignment means changing a reference to point to another object.

When you reassign, the old object may become unreachable if no other reference is pointing to it.

✅ Example:

java
Copy
Edit
class Student {}

public class Test {
    public static void main(String[] args) {
        Student s1 = new Student(); // s1 --> object1
        Student s2 = new Student(); // s2 --> object2

        s1 = s2;  // Now s1 points to object2; object1 is unreferenced
    }
}
🔵 What happens here?


Step	Action
1	s1 points to object1
2	s2 points to object2
3	s1 = s2; => now both s1 and s2 point to object2
4	object1 has no reference anymore → eligible for garbage collection
3. 📌 Garbage Collection
Java has an Automatic Garbage Collector.

It removes unused objects (objects with no reference) from memory.

Helps in freeing up memory and preventing memory leaks.

✅ Key Points:

You cannot force garbage collection, but you can request it using:

java
Copy
Edit
System.gc();
JVM decides when to actually run it.

4. 📌 finalize() Method (before garbage collection)
finalize() is a special method that is called before the object is garbage collected.

You can override it to do cleanup operations like closing files or releasing resources.

✅ Example:

java
Copy
Edit
class Student {
    protected void finalize() {
        System.out.println("Finalize method called");
    }
}

public class Test {
    public static void main(String[] args) {
        Student s = new Student();
        s = null;  // Now object is eligible for garbage collection

        System.gc();  // Request JVM to run Garbage Collector
    }
}
🔵 Output:

sql
Copy
Edit
Finalize method called
⚡ Important:

finalize() is called only once before the object is destroyed.

In Java 9+, finalize() is deprecated (because it's slow and error-prone).

In modern Java, better to use try-with-resources or explicit resource handling.
