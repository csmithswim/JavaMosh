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

Get request - limited amount of data can be sent.

Post request - large amount of data can be sent.

Session is a conversational state between client and server and it can consist of multiple request and response between client and server.

Since HTTP and web server both are stateless, the only way to maintain a session is when some unique information aboute the session (session id) is passed between server and client in every request and response.

Servlet config object represent single servlet.

Servletcontext represents whole web application running on particular JVM and common for all the servlet.

There are 5 stages of a servlet: servlet is loaded, instantiated, initialized, service the request, and servlet is destroyed.

RequestDispatcher interface is used to foward the request to another resource that can be HTML, JSP or another servlet in same application.

We can also use this to include the content of another resource to the response.

There are two methods defined in this interface:
1. void foward()
2. void include()

Cookies are text data sent by server to the client and it gets saved at the client local machine.
Servlet API provides cookies support through javax.servlet.http.Cookie class that implements Serializable and Cloneable interfaces.
HttpServletRequest getCookies() method is provided to get the array of Cookies form request, since there is no point of adding Cookie to request, there are no methods to set or add cookie to request. Similarly httpservletresponse addcookie(cookie c) method is provided to attach cookie in response header, there are no getter methods for cookie.

JDBC Driver is a software component that enables java application to interact with the database. There are 4 types of JDBC drivers: 
JDBC-ODBC bridge driver
Native-API driver (partially java driver)
Network protocol driver (fully java driver)
Thin driver (fully java driver)

There are 5 steps to do when you connect to the database in Java: 

Registering the driver class
Creating connection
Creating statement
Executing queries
Closing connection

Make sure you close your connection finally.

Interfaces in JDBC: COnnection, statement, prepared statement, resuletset, resultset/metadata, database metadata, callable statement.

Class in JDBC: driver manager, blob, clob, types, SQL exception.

JDBC connection interface - the one that maintains the session with the database. It can be used for transation management.

executeQuery() - this method is used to execute the SQL statements which retrive some data from the database.

executeUpdate() - this method is used to execute the SQL statements which update or modify the database.

execute() - this method can be used for any kind of SQL statements.

