# Week-7
**Note:** Before starting Learn the basic of [java](https://www.w3schools.com/java/)

## Memory Locations For Variables & Java

## Memory Management & Java
For most part of memory management there are static and dynamic parts
- static - global data, compiled codes, runtime system.
- dynamic - runtime stack and heap 

**What is a stack?**

The stack is a LIFO (Last-In-First-Out) data structure. manage using push and pop.

In the stack, as you said, things are "separated" and you can only get at whatever's on top. The operating system uses a stack to manage local variables in functions and procedures. Let's imagine you have a function in a function in a function (let's say f1() calls f2() which in turn calls f3() ):

When the first function (f1) is executed, you have its variables available; when that function calls another, all of f1's variables get pushed into the stack and the new function's variables (f2) take over. When THAT function calls f3, it is f2's variables that get pushed into the stack. 

**Advantage**
- fast
_ auto manged by the progam (function)
**Disadvantage**
- manage by program not the dev (so not flexible)

**What is a heap?**

The heap stores dynamic memory values that are requested on runtime. In additon, programmer needs to maintain the memory. Not fast, but durable across function calls

**Advantage** 
- manage the dev (flexible)
**Disadvantage**
- time in execution( not fast)
- memory leak
- buffer overflow 

Using the the language in C++ heap is call using **malloc or memory allocation**. 

It is basically asaking the system for the amount of memory is asked for and return a pointer to the starting address. Thus freeing up the memory, 
which it can be use for other purposes.

Automatic memory management works by the process of **Garbage collection or GC**. GC takes place by pausing the execution and going through the whole program to free up unused memory blocks. The advantage of this is that it keep the  module cleaner(fewer  bugs)

A **dangling pointer** is a pointer that points to invalid data or to data which is not valid anymore

A **memory leak** is when a user ask for memory that was never freed

**What is execption?**

An **exception** is an event, which occurs during the execution of a program, that disrupts the normal flow of the program's instructions

Example of this
![exception](exception.png)

**Checked vs. Unchecked Exceptions** 
- uncheck are exceptions that do not have to be caught by an explicit try/catch block. These typically represent unrecoverable errors or unforseen/unplannable exceptions
- check are exception that you have to catch with an explicit try/catch block if they could be thrown. Typically, these are common errors that you should be able to know how to handle or recover from.


## Parameter 
