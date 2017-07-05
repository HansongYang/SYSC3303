Assignment Requirement:
Background
In this problem we are going to simulate a database using a BoundedBuffer (as in the example studied in the lectures). We will have threads that read from the database and threads that write to a database. This is a classic thread problem called the Readers Writers problem. 
You have been provided with four Java files: 
ReadWrite0.java 
Database.java 
Reader.java 
Writer.java 
These files implement "version 0" of the Readers Writers problem and allow just one thread (i.e. one reader or one writer) to access the 
database at a time. 

Part 1
Modify the java files provided to implement "version 1" of the Readers Writers problem. In version 1, any number of readers may access the 
database at the same time, but just one writer may access the database at once. (And readers and writers may not access the database at the 
same time.) This implementation favours readers (and writers could starve). 

Part 2
Modify the java files provided (or your solution to part 1) to implement "version 2" of the Readers Writers problem. In version 2 the same 
rules apply as in version 1, i.e. any number of readers may access the database at the same time, but just one writer may access the database 
at once. (And readers and writers may not access the database at the same time.) In addition, writers must not be kept waiting any longer than 
absolutely necessary. Thus, if a writer is waiting to write, no other readers may start reading. This implementation favours writers (and 
readers could starve).
 
Part 3
Modify the java files provided (or your solution to part 1 or 2) to implement "version 3" of the Readers Writers problem. In version 3 the same 
rules apply as in version 1, i.e. any number of readers may access the database at the same time, but just one writer may access the database at
once. (And readers and writers may not access the database at the same time.) In addition, neither readers nor writers can be permitted to 
starve. This solution must favour neither readers nor writers. Note that your solution must not use a queue or any other list-like mechanism, 
just Java's mutual exclusion and condition synchronization, as discussed in the lectures. 

Work Products
Create three folders part1, part2, and part3. Each folder will contain the work products of that part of your solution. 
In each folder ensure that you have the following: 
A “README.txt” file explaining the names of your files, set up instructions, etc. 
One UCM showing all components in your system. 
A UML Collaboration diagram of your system. 
A UML Class diagram of your system. 
The source code for your solution. Your code should demonstrate good programming style, be well documented, etc. For examples of "industrial quality" Java code, have a look at Sun's Java coding conventions, which can be found on our Java resources Web site. (This site can be reached by a link from the SYSC 3303 Web site.) 

Files:

1.Version 1: Database1.java
	     Reader1.java
	     Writer1.java
	     ReadWrite1.java

2.Version 2: Database2.java
	     Reader2.java
	     Writer2.java
	     ReadWrite2.java

3.Version 3: Database3java
	     Reader3.java
	     Writer3.java
	     ReadWrite3.java