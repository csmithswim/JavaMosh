JVM - Java Virtual Machine - an abstract machine specificationt hat provides runtime environment in which java bytecode can be executed.
JRE(Java Runtime Environment) is a runtime environment which implements JVM and proviced all class libraries and other files that JVM uses at runtime.
JDK(Java Development Kit) is the tool necessary to compile, document and package Java programs. The JDK completely includes JRE.

JVM>JRE>JDK

Synchronization - a process which keeps all concurrent threads in execution to be in sync. It avoids memory consistency errors caused to to inconsistent view of shared memory.

Process - an executing instance of a program is called a process.

A thread is a subset of the process. Runs within the processes, and processes are running on top of operating systems.

Threads are controlled by programmers in the program, process is controlled by OS.

Processes are independent and threads are dependent.

Wrapper class - How to convert the primitive types to reference types. Known as boxing and autoboxing.

You can extract the value of objects with unboxing.

Final - used to apply restrictions on class, method and variable.
Final class can't be inherited, final method can't be overriden and final variable value can't be changed.

Finally is used to place important code, it will be executed whether exception is handled or not. Used commonly in try/catch blocks.

Finalize is used to perform clean up processing just before object is garbage collected.

StringBuffer operations are thread-safe and synchronized where StringBuilder operations are not thread-safe.

Buffer/Builder are mutable. 

StringBuffer is to be used when multiple threads are working on same String and StringBuilder in the single threaded environment.

StringBuilder performance is faster when compared to StringBuffer because of no overhead of synchronized.

Both stack and heap are apart of RAM.

Stack - stack memory is used only by one thread of execution. Objects are located by hexadecimal in the stack and also point to a different number in the stack.

Stack contains object, heap contains attributes and methods.

Heap - Memory is used by all the parts of the application. Where we use the new operator that is constructed dynamically in runtime. 

Array list is not synchronized. 
Vector is synchronized. 

Hashmap is a non synchronized and are not thread safe.
Hashtable is synchronized. It is thread-safe and can be shared with many threads.

Equals() method is defined Object class Java and used for checking equality of two objects defined by business logic.

== or equality operator in Java is a binary operator provided by Java programming language and used to compare primitives and objects.

Abstract class can provide complete, default code and/or just the details that have to be overriddden.

An interface cannot provide any code at all, just the signature.

Polymorphism is briefly described as "one interface, many implementations".

It is characteristic of being able to assign a different meaning or useage to something in different contexts.

Runtime polymorphism is a process in which a call to an overriden method is resolved at runtime rather than at compile-time. In this process, an overriden method is called through the reference variable of a superclass. The determination of the method to be called is based on the object being referred to by the refgerence variable.

Overloaded method - methods of the same class shares the same name but each method must have different number of parameters or parameters having different types and order.
Compile time polymorphism

Overriden method - sub class have the same method with same name and exactly the same number and type of parameters and same return type as a super class.
Run time polymorphism

A private method cannot be overriden since it is not visible from any other class.

If you create a similar method with the same return type and same method arguements in child class then it will hdie the superclass method; this is known as method hiding.

Java does not support multiple inheritance.

Servlets are part of the enterprise edition of java.

It is server side technologies to extend the capability of web servers by providing support for dynamic response and data persistence.
The javax.serlet and javax.servglet.http packagews provide interfaces and classes for writing our own servlets.
All servlets must implment the javax.servlet.Servlet interface, which defines servlet lifecycle methods. As most web applications are accessed using HTTP protocol, we mostly extend Httpservlet class. Servlet API hierachy.

