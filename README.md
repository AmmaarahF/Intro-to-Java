# Intro-to-Java

What is Java ?
---------------------------
- Java forms part of Back-End Web development.
- Java is widely-used, general-purpose, class-based, and object-oriented programming language that is designed to have as few implementation dependencies as possible.
- <b>Java Runtime Environment (JRE)</b> for operation. This component enables your computer to run Java programs.
- <b>Java Development Kit (JDK)</b> for crafting and compiling Java programs, bundled with the JRE and handy compilers and tools. <b>WITH JDK INSTALLATION, THE JRE COMES ALONG WITH IT</b>
- In Java, "compile" refers to the process of converting the source code written in Java into bytecode that can be executed by the Java Virtual Machine (JVM). This process involves several steps and is carried out by the Java compiler, which is part of the Java Development Kit (JDK).

Installing JDK
--------------------------
- https://www.oracle.com/java/technologies/downloads/
- Java JDK link

Java Variables
-------------------------
- <b>Dynamically Typed</b> - Variable types are determined at runtime through context in the code.
- <b>Statically Typed</b> - Variables types must be declared before the program can be compiled.

Declaring a variable 
-------------------------
eg. var isWaterWet = true;
    int five;

Decision Structures in Java
--------------------------------
- if statements - The if statement works like a side road in the program. If a certain situation happens, the program takes that side road and executes a certain block of code, then it goes back to the main path of execution.

- If-else Statements - The if-else statement is a decision structure that allows a program to take one of two paths, depending on whether a certain condition is met.

- If-Else-If Statements - The if-else-if statement is a versatile tool that can be used to control the flow of a program. It can be used to execute different code blocks based on multiple conditions.

Switch Statements
-----------------------------
- The switch statement works like the if-else-if decision structure, perfect for situations with more than two options. The key distinction is that if-else-if checks conditions, while the switch statement checks for equality.

Switch Expressions
----------------------------
- Switch expressions are like switch statements, but they are more convenient. Instead of separately declaring a message and then assigning it with a switch statement, you can simplify things with switch expressions.
- eg, System.out.println("Enter grade");
<br>
      String message = switch(grade){
         case "A" , "B" -> "Exellent job!";
         case "C" -> "Good job!";
         case "D" -> "You need to work a bit harder";
         case "F" -> "Uh oh!";
         default -> "Error. Invalid grade";
  };


<br>

Relational Operators
-------------------------------
- Relational operators are these symbols that you use when you are dealing with conditions.
- eg, > , <, >= , <= , == , !=


Logical Operators
-----------------------------
- Logical operators let you mix and match conditions to give you one clear yes or no answer, like a Boolean value. They come in handy when you have tricky requirements for making decisions.
- eg., && , || , and !


Short Circuit Logic
------------------------------
- The 'and' and 'or' logical operators help us combine two conditions into one. When we use 'and,' both conditions must be true. If the first condition is false, there is no need to check the second one because both have to be true for the whole thing to be true.
- When using the && operator , if one condition is false, the the entire condiion is false.
- When using the || operator, if one is True then the entur confition is true.
- with 'or,' if the first condition is true, there is no need to bother with the second condition.


Repetition Structures in Java
--------------------------------
- While Loop
  > Runs the code over and over until the condition is met.
- Do While Loop
  > Loop that executes, then checks the condition to determine whether to repeat.
- For Loop
  > Loop that executes a specified number of times.
- Nested Loops
  > Loops inside of loops
- Break Statement
  > A break statement will end a loop no matter what iteration it's on.

<br>

Methods in Java
---------------------------------
- Creating Methods
  > eg., public static int calculateSum(int num1, int num2){
      int sum = num1 + num2;
      return sum;
  }

Variable Scope
--------------------------------
- Variables are only valid within the scope in which they were defined.

Objects in Java
--------------------------------
