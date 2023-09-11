
Chapter 1  Computer Programming
===============================
This book is your guide to thinking like a computer scientist, a way of approaching problems that draws from mathematics, engineering, and natural science. Let's break down what that means:

1.  **Mathematics:** Computer scientists use **formal languages**, such as programming languages, to convey ideas in a structured and unambiguous way. It's like specifying the dimensions and materials when you're building a house; every detail matters.

2.  **Engineering:** We are also designers at heart, assembling pieces of code or hardware to create functioning systems. We evaluate trade-offs between different solutions, deciding what is the most effective way to build our digital "machines."

3.  **Natural Science:** Observation and experimentation are key. We observe how complex systems---like a computer network or a software application---behave, form hypotheses about them, and then test our ideas.

4.  **Philosophy:(( Here, we tackle the "why" and the "what if" questions. Philosophy teaches us to think critically and question assumptions. For instance, is the most efficient algorithm always the best choice, or are there ethical considerations? And what does it mean for computers to "think" in the context of artificial intelligence? It helps us understand the broader implications of our work, and approach problems that we don't (yet) a good understanding of.

Armed with this multidisciplinary approach, one of the most crucial skills you'll develop is problem-solving. Think of it as a multi-step journey. First, you identify what you're up against; this is called formulating problems. It's like diagnosing an illness before you can treat it. Then, you brainstorm various treatments or solutions, which is thinking creatively about solutions. Finally, you write a prescription or lay down a course of action, and this is expressing solutions clearly and accurately.

Learning to program, perhaps in Java for this course, serves dual purposes. On the surface, you're learning a valuable skill that's akin to learning how to assemble a car engine. But deeper than that, you're also learning how to think systematically and solve problems---skills that will serve you well in any endeavor. Programming becomes not just an end, but a means to enrich your ability to think, question, and solve. As we delve further into the material, you'll find that the act of coding is just one piece of a much larger puzzle.

1.1  What Is a Computer?
------------------------
A **computer** is a machine designed to process information. It's a bit like a very obedient dog that can perform tricks, solve problems, and follow commands, but it does so by crunching numbers and following instructions known as algorithms. The heart of a computer lies in its hardware and software.

**Hardware** refers to the physical components that you can touch: the **Central Processing Unit (CPU)((, which is the brain of the computer; **memory**, which is the computer's short-term and long-term storage; and other parts like the monitor, keyboard, solid state drives, and mouse. Think of the CPU as the dog's brain, constantly processing commands. Memory is like the dog's ability to remember commands and tricks. These components work together in a harmonious dance to get tasks done.

**Software**, on the other hand, is a set of instructions that tells the hardware what to do. Imagine teaching your dog new tricks; the commands you use are like the software. The CPU takes these instructions from the software and executes them, using the memory to store and retrieve information as needed.

There are different types of computers, each with its own specialized use. Desktop computers are the kind you might have at home or at work, good for a wide range of tasks from writing emails to playing video games. Laptops are portable versions of desktops. Then there are servers, which are like librarians that manage vast amounts of data and allow many people to access it. Finally, we have supercomputers, which are like Olympic athletes, designed for highly specialized tasks that require enormous amounts of calculation, such as weather forecasting or scientific research.

The history of computers is a fascinating journey that starts from basic calculating machines in ancient times to the modern, powerful machines we use today. Imagine the first computers as being like the wheel---a revolutionary invention but quite basic compared to what we have now. Over time, computers have evolved from room-sized behemoths to devices that can fit in the palm of your hand, much like how transportation evolved from horse-drawn carriages to cars and airplanes.

> * * * * *
>
> ![](https://greenteapress.com/thinkjava7/html/thinkjava2_001.png)    ![](https://greenteapress.com/thinkjava7/html/thinkjava2_002.png)
>
> | Figure 1.1: Example processor and memory hardware. |
>
> * * * * *


1.2  What Is Programming?
-------------------------
A **program** is like a recipe for a computer. It lays out step-by-step what the computer should do. Just like you might follow a recipe to bake a cake, a computer follows a program to perform a specific task. A program is made of instructions, which are the individual steps that the computer takes to achieve its goal. These instructions are executed on the computer hardware, specifically by the Central Processing Unit (CPU).

Different programming languages---like English, French, or Spanish for humans---have their own ways of expressing these instructions, but most languages share a few basic types of instructions:

1.  **Input:** This is like asking someone for an ingredient while cooking. The computer collects data from somewhere---maybe a keyboard, a file, or a sensor.

2.  **Output:** Imagine you've finished baking your cake and now you're showing it off. This is what the computer does when it displays data on a screen, saves it to a file, or sends it to another device.

3.  **Math:** These are your basic kitchen calculations. Need to half a recipe? That's division. Doubling it? That's multiplication. The computer performs basic mathematical operations like these to process data.

4.  **Decision:** Think of this as choosing whether to bake a cake or cookies based on what ingredients are available. The computer checks conditions---like if a number is zero, or if a button has been pressed---and then decides what to do next.

5.  **Repetition:** Imagine stirring cake mix. You don't just do it once; you do it repeatedly until it's ready. In the same way, computers can repeat an action until a certain condition is met.

The magic happens when these simple instructions are combined in clever ways. Take Google's search engine. It's a complex system, but at its core, it's using these basic types of instructions to sift through an enormous amount of data. It uses input to get your search query, performs math and decision-making to find relevant results, and then gives you an output by displaying them. All the while, repetition is used to keep refining these tasks.

In essence, programming is the art of taking a big, complicated task and breaking it down into smaller parts that the computer can handle. It's a bit like building a house. You don't just slap it together; you lay one brick at a time. And just as you wouldn't use a single hammer for every job on a construction site, complex tasks often require various types of these basic instructions, combined and sequenced in specific ways to get the job done.

1.3  The Hello World Program
----------------------------

Traditionally, the first program you write when learning a new programming language is called the "Hello World" program. It outputs the words Hello, World! to the screen. In Java, it looks like this:
```java
public class Hello {
  public static void main(String[] args) { 
	// generate some simple output
	System.out.println("Hello, World!");
}
}
```

When this program runs, it displays the following:

`Hello, World!`

Notice that the output does not include the quotation marks.

Java programs are made up of *class* and *method* definitions, and methods are made up of *statements*. A statement is a line of code that performs a basic action. In the Hello World program, this line is a print statement that displays a message to the user:

` System.out.println("Hello, World!"); `

`System.out.println` displays results on the screen; the name `println` stands for "print line". Confusingly, *print* can mean both "display on the screen" and "send to the printer". In this book, we'll try to say "display" when we mean output to the screen. Like most statements, the print statement ends with a semicolon (`;`).

Java is "case-sensitive", meaning that uppercase and lowercase are different. In the Hello World program, `System` has to begin with an uppercase letter; `system` and `SYSTEM` won't work.

A **method** is a named sequence of statements. This program defines one method named `main`:

` public static void main(String[] args) `

The name and format of `main` is special: when the program runs, it starts at the first statement in `main` and ends when it finishes the last statement. Later, you will see programs that define more than one method.

This program defines a class named `Hello`. For now, a class is a collection of methods; we'll have more to say about this later. You can give a class any name you like, but starting with a capital letter is conventional. The name of the class has to match the name of the file it is in, so this class has to be in a file named Hello.java.

Java uses curly braces (`{` and `}`) to group things together. In Hello.java, the outermost braces contain the class definition, and the inner braces contain the method definition.

The line that begins with two slashes (`//`) is a comment, a bit of English text explaining the code. When Java sees `//`, it ignores everything from there until the end of the line. Comments do not affect the execution of the program, but they make it easier for other programmers (and your future self) to understand what you meant to do.

1.4  Compiling Java Programs
----------------------------

The programming language you will learn in this book is **Java**, which is a high-level language. Other high-level languages you may have heard of include Python, C and C++, PHP, Ruby, and JavaScript.

Before they can run, programs in high-level languages have to be translated into a low-level language, also called "machine language". This translation takes some time, a small disadvantage of high-level languages. But high-level languages have two major advantages:

-   It is *much* easier to program in a high-level language. Programs take less time to write, are shorter and easier to read, and are more likely to be correct.
-   High-level languages are **portable**, meaning they can run on different kinds of computers with few or no modifications. Low-level programs can run on only one kind of computer.

Two kinds of programs translate high-level languages into low-level languages: interpreters and compilers. An interpreter reads and executes a high-level program, meaning it does what the program says. It processes the program a little at a time, alternately reading lines and performing computations. Figure [1.2](https://greenteapress.com/thinkjava7/html/chapter-01.html#fig.interpreter) shows the structure of an interpreter.

> * * * * *
>
> ![](https://greenteapress.com/thinkjava7/html/thinkjava2_003.png)
>
> | Figure 1.2: How interpreted languages are executed. |
>
> * * * * *

In contrast, a compiler reads the entire program and translates it ultimately before the program starts running. The high-level program is called the source code. The translated program is called the object code, or the executable. Once a program is compiled, you can execute it repeatedly without further translation of the source code. As a result, compiled programs often run faster than interpreted programs.

Note that object code, as a low-level language, is not portable. For example, you cannot run an executable compiled for a Windows laptop on an Android phone. To run a program on different types of machines, it must be compiled multiple times. It can be difficult to write source code that compiles and runs correctly on different types of machines.

To address this issue, Java is *both* compiled and interpreted. Instead of translating source code directly into an executable, the Java compiler generates code for a virtual machine. This "imaginary" machine has the functionality common to desktops, laptops, tablets, phones, etc. Its language, called Java byte code, looks like object code and is easy and fast to interpret.

As a result, it's possible to compile a Java program on one machine, transfer the byte code to another machine, and run the byte code on that other machine. 

Figure [1.3](https://greenteapress.com/thinkjava7/html/chapter-01.html#fig.compiler) shows the steps of the development process. 

The Java compiler is a program named javac. It translates .java files into .class files that store the resulting byte code. The Java interpreter is another program, named java, which is short for "Java Virtual Machine" (JVM).

> * * * * *
>
> ![](https://greenteapress.com/thinkjava7/html/thinkjava2_004.png)
>
> | Figure 1.3: The process of compiling and running a Java program. |
>
> * * * * *

The programmer writes source code in the file Hello.java and uses javac to compile it. If there are no errors, the compiler saves the byte code in the file Hello.class. To run the program, the programmer uses java to interpret the byte code. The result of the program is then displayed on the screen.

Although it might seem complicated, these steps are automated in most development environments. Usually, you only have to press a button or type a single command to compile and interpret your program. On the other hand, it is important to know what steps are happening in the background, so if something goes wrong you can figure out what it is.

1.5  Displaying Two Messages
----------------------------

You can put as many statements as you like in the `main` method. For example, to display more than one line of output:

```java
public class Hello2 {
  public static void main(String[] args) {
    // generate some simple output
    System.out.println("Hello, World!"); // first line
    System.out.println("How are you?"); // another line
}
}
```

As this example also shows, you can put comments at the end of a line as well as on lines all by themselves.

Phrases that appear in quotation marks are called strings, because they contain a sequence of characters strung together in memory. Characters can be letters, numbers, punctuation marks, symbols, spaces, tabs, etc.

`System.out.println` appends a special character, called a newline, that moves to the beginning of the next line. If you don't want a newline at the end, you can use `print` instead of `println`:

```java
public class Goodbye {
  public static void main(String[] args) {
    System.out.print("Goodbye, ");
    System.out.println("cruel world");
}
}
```

In this example, the first statement does not add a newline, so the output appears on a single line:

` Goodbye, cruel world `

Notice that there is a space at the end of the first string, which appears in the output just before the word cruel.

1.6  Formatting Source Code
---------------------------

In Java source code, some spaces are required. For example, you need at least one space between words, so this program is not legal:

```java
publicclassGoodbye{
  publicstaticvoidmain(String[] args) {
  System.out.print("Goodbye, ");
  System.out.println("cruel world"); } }
```

But most other spaces are optional. For example, this program *is* legal:

```java
  public class Goodbye {
    public static void main(String[] args) {
    System.out.print("Goodbye, ");
    System.out.println("cruel world"); } }
```

The newlines are optional, too. So we could just write this:

```java
  public class Goodbye { public static void main(String[] args) { System.out.print("Goodbye, "); System.out.println
  ("cruel world");}}
```

It still works, but the program is getting harder and harder to read. Newlines and spaces are important for visually organizing your program, making it easier to understand the program and find errors when they occur.

Many editors will automatically format source code with consistent indenting and line breaks. For example, in DrJava, you can indent your code by selecting all text (Ctrl+A) and pressing the Tab key.

Organizations that do a lot of software development usually have strict guidelines on how to format source code. For example, Google publishes its Java coding standards for use in open source projects: <https://google.github.io/styleguide/javaguide.html>.

You probably won't understand these guidelines now, because they refer to language features you haven't yet seen. But you might want to refer to them periodically as you read this book.

1.7  Using Escape Sequences
---------------------------

It's possible to display multiple lines of output with only one line of code. You just have to tell Java where to put the line breaks:

```java
  public class Hello3 {
    public static void main(String[] args) {
    System.out.print("Hello!\nHow are you doing?\n");
} }
```

The output is two lines, each ending with a newline character:

` Hello! How are you doing? `

Each `\n` is an escape sequence, or two characters of source code that represent a single character. (The backslash allows you to *escape* the string to write special characters.) Notice there is no space between `\n` and `How`. If you add a space there, there will be a space at the beginning of the second line.

Java has a total of eight escape sequences. The most commonly used include the following:

| Escape Character | Description |
| --- | --- |
| `\\` | Backslash; used to escape other characters |
| `\"` | Double quote; used to include quotes within strings |
| `\'` | Single quote; used within character literals |
| `\n` | Newline; moves the cursor to the next line |
| `\t` | Tab; inserts a horizontal tab |

 For example, to write quotation marks inside of strings, you need to escape them with a backslash:

```java
  System.out.println("She said \"Hello!\" to me.");
```

The result is as follows:

` She said "Hello!" to me. `

1.8  What Is Computer Science?
------------------------------

This book intentionally omits some details about the Java language (such as the other escape sequences), because our main goal is teaching you how to think like a computer scientist. Being able to understand computation is much more valuable than just learning how to write code.

If you're interested in learning more about Java itself, Oracle maintains an official set of tutorials on its website (<https://thinkjava.org/tutorial>). The "Language Basics" tutorial, found under "Learning the Java Language", is a good place to start.

One of the most interesting aspects of writing programs is deciding how to solve a particular problem, especially when there are multiple solutions. For example, there are numerous ways to sort a list of numbers, and each way has its advantages. In order to determine which way is best for a given situation, we need techniques for describing and analyzing solutions formally.

An **algorithm** is a sequence of steps that specifies how to solve a problem. Some algorithms are faster than others, and some use less space in computer memory. Computer science is the science of algorithms, including their discovery and analysis. As you learn to develop algorithms for problems you haven't solved before, you will learn to think like a computer scientist.

Designing algorithms and writing code is difficult and error-prone. For historical reasons, programming errors are called bugs, and the process of tracking them down and correcting them is called debugging. As you learn to debug your programs, you will develop new problem-solving skills. You will need to think creatively when unexpected errors happen.

Although it can be frustrating, debugging is an intellectually rich, challenging, and interesting part of computer science. In some ways, debugging is like detective work. You are confronted with clues, and you have to infer the processes and events that led to the results you see. Thinking about how to correct programs and improve their performance sometimes even leads to the discovery of new algorithms.

1.9  Debugging Programs
-----------------------

It is a good idea to read this book in front of a computer so you can try out the examples as you go. You can run many of the examples directly in DrJava's Interactions pane (see Appendix [A.2](https://greenteapress.com/thinkjava7/html/appendix-a.html#interactions)). But if you put the code in a source file, it will be easier to try out variations.

Whenever you are experimenting with a new feature, you should also try to make mistakes. For example, in the Hello World program, what happens if you leave out one of the quotation marks? What if you leave out both? What if you spell `println` wrong? These kinds of experiments help you remember what you read. They also help with debugging, because you learn what the error messages mean. It is better to make mistakes now and on purpose than later on and accidentally.

Debugging is like an experimental science: once you have an idea about what is going wrong, you modify your program and try again. If your hypothesis was correct, then you can predict the result of the modification, and you take a step closer to a working program. If your hypothesis was wrong, you have to come up with a new one.

Programming and debugging should go hand in hand. Don't just write a bunch of code and then perform trial-and-error debugging until it all works. Instead, start with a program that does *something* and make small modifications, debugging them as you go, until the program does what you want. That way, you will always have a working program, and isolating errors will be easier.

A great example of this principle is the Linux operating system, which contains millions of lines of code. It started out as a simple program Linus Torvalds used to explore the Intel 80386 chip. According to Larry Greenfield in The Linux Users' Guide, "One of Linus's earlier projects was a program that would switch between printing AAAA and BBBB. This later evolved to Linux."

Finally, programming sometimes brings out strong emotions. If you are struggling with a difficult bug, you might feel angry, despondent, or embarrassed. Remember that you are not alone, and virtually every programmer has had similar experiences. Don't hesitate to reach out to a friend and ask questions!

1.11  Vocabulary
----------------

Throughout the book, we try to define each term the first time we use it. At the end of each chapter, we include the new terms and their definitions in order of appearance. If you spend some time learning this vocabulary, you will have an easier time reading the following chapters.

| Term | Description |
| --- | --- |
| Problem Solving | The process of formulating a problem, finding a solution, and expressing the solution. |
| Hardware | The electronic and mechanical components of a computer, such as CPUs, RAM, and hard disks. |
| Processor | A computer chip that performs simple instructions like basic arithmetic and logic. |
| Memory | Circuits that store data as long as the computer is turned on. Not to be confused with permanent storage devices like hard disks and flash. |
| Program | A sequence of instructions that specifies how to perform tasks on a computer. Also known as "software". |
| Programming | The application of problem solving to creating executable computer programs. |
| Statement | Part of a program that specifies one step of an algorithm. |
| Print Statement | A statement that causes output to be displayed on the screen. |
| Method | A named sequence of statements. |
| Class | A collection of related methods. 
| Comment | A part of a program that contains information about the program but has no effect when the program runs. |
| High-level Language | A programming language that is designed to be easy for humans to read and write. |
| Low-level Language | A programming language that is designed to be easy for a computer to run. Also called "machine language". |
| Portable | The ability of a program to run on more than one kind of computer. |
| Interpret | To run a program in a high-level language by translating it one line at a time and immediately executing the corresponding instructions. |
| Compile | To translate a program in a high-level language into a low-level language, all at once, in preparation for later execution. |
| Source Code | A program in a high-level language, before being compiled. |
| Object Code | The output of the compiler, after translating the program. |
| Executable | Another name for object code that is ready to run on specific hardware. |
| Virtual Machine | An emulation of a real machine. The JVM enables a computer to run Java programs. |
| Byte Code | A special kind of object code used for Java programs. Byte code is similar to object code, but it is portable like a high-level language. |
| String | A sequence of characters; the primary data type for text. |
| Newline | A special character signifying the end of a line of text. Also known as "line ending", "end of line" (EOL), or "line break". |
| Escape Sequence | A sequence of code that represents a special character when used inside a string. |
| Algorithm | A procedure or formula for solving a problem, with or without a computer. |
| Computer Science | The scientific and practical approach to computation and its applications. |
| Bug | An error in a program. |
| Debugging | The process of finding and removing errors. |


1.12 Signing Up for Repl.it and Running Your First Java Program
---------------

Before diving into the fascinating world of Java programming, you'll need an environment where you can write and run code. While there are various ways to do this, for this class, I highly recommend using Repl.it. It's a beginner-friendly, web-based integrated development environment (IDE) that requires no installation. You can write, compile, and run your Java programs all in one place.

#### Steps to Get Started

1.  Open your web browser and navigate to [Repl.it](https://replit.com/). 

2.  Click on the "Sign Up" button usually found at the top-right corner of the page. You'll be prompted to enter your email, create a username, and set a password. Follow the instructions, and you'll have your account set up in no time.

3.  After signing up, check your email for a confirmation link from Repl.it. Click on the link to activate your account. If you don't see the email, make sure to check your spam folder.

4.  Once your account is activated, return to Repl.it and log in using the credentials you just created.

5.   After logging in, you'll be taken to your dashboard. Here, you can create a new Repl by clicking the "+ New Repl" button usually found at the top. A dialog will appear asking you to select the programming language. Type in or scroll down to find "Java" and select it.

6.  You'll also have an option to name your Repl; you can name it something like `MyFirstJavaProgram` or leave it as the default name. Once you're ready, click "Create Repl" to proceed.

7.  You should now see a split screen. On the left side is where you'll write your Java code, and on the right side is the output window. The editor will usually have a template code like:

 ```java
    `public class Main {
        public static void main(String[] args) {
            System.out.println("Hello world!");
        }
    }
   ```

  Feel free to leave this as is for your first program.

8.  To **compile** your java code, you'll go the "Console" window, and type `javac Main.java` (or whatever your java file is called).
9. Once the file has been compiled, you **run** the program by typing `java Main` (or whatever your java file is called).
10. You can can also use the **Run** button to run code. However, you need to aware that this will compile and run ALL java files that you have saved.  (So, this can sometimes cause problems!) 

11.   Repl.it automatically saves your work, so there's no need to worry about losing your code.

#### Congratulations!

You've just written and run your first Java program using Repl.it. As you progress through this course, we'll be using this platform frequently to build and test various Java programs. Happy coding!


1.13 Exercises
---------------

At the end of each chapter, we include exercises you can do with the things you've learned. We encourage you to at least attempt every problem. You can't learn to program only by reading about it; you have to practice. Here, for the coding questions, you should open up repl.it and create your own programs.


### Exercise 1  

Computer scientists have the annoying habit of using common English words to mean something other than their common English meanings. For example, in English, statements and comments are the same thing, but in programs they are different.

1.  In computer jargon, what's the difference between a statement and a comment?
2.  What does it mean to say that a program is portable?
3.  In common English, what does the word compile mean?
4.  What is an executable? Why is that word used as a noun?

The vocabulary section at the end of each chapter is intended to highlight words and phrases that have special meanings in computer science. When you see familiar words, don't assume that you know what they mean!

### Exercise 2  

Before you do anything else, find out how to compile and run a Java program. Some environments provide sample programs similar to the example in Section 1.3.

1.  Type in the Hello World program; then compile and run it.
2.  Add a print statement that displays a second message after the Hello, World!. Say something witty like, How are you?. Compile and run the program again.
3.  Add a comment to the program (anywhere), recompile, and run it again. The new comment should not affect the result.

This exercise may seem trivial, but it is the starting place for many of the programs we will work with. To debug with confidence, you will need to have confidence in your programming environment.

In some environments, it is easy to lose track of which program is executing. You might find yourself trying to debug one program while you are accidentally running another. Adding (and changing) print statements is a simple way to be sure that the program you are looking at is the program you are running.

### Exercise 3  

It is a good idea to commit as many errors as you can think of, so that you see what error messages the compiler produces. Sometimes the compiler tells you exactly what is wrong, and all you have to do is fix it. But sometimes the error messages are misleading. Over time you will develop a sense for when you can trust the compiler and when you have to figure things out yourself.

Starting with the Hello World program, try out each of the following errors. After you make each change, compile the program, read the error message (if there is one), and then fix the error.

1.  Remove one of the opening curly braces.
2.  Remove one of the closing curly braces.
3.  Instead of `main`, write `mian`.
4.  Remove the word `static`.
5.  Remove the word `public`.
6.  Remove the word `System`.
7.  Replace `println` with `Println`.
8.  Replace `println` with `print`.
9.  Delete one parenthesis.
10. Add an extra parenthesis.
