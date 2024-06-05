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
- objects are like containers holding data and actions.


Java Constructors
----------------------------------
- Java constructors initialize new objects.
- They have the same name as the class and no return type.
- eg., public Dog(String name) {<br>
        this.name = name;<br>
    }


Object Instantiation
----------------------------------
- Object instantiation in Java involves creating a new instance of a class using the new keyword, which calls the class's constructor.
-  public Car(String model) {<br>
        this.model = model;<br>
    }
- eg., Rectangle room1 = new Rectangle();

Method Parameters as Objects
--------------------------------------
- In Java, you can pass objects as parameters to methods, allowing the method to operate on the object's attributes and methods
- eg., public Book(String title) { //constructor<br> 
        this.title = title;<br>
    }
<br>
    // Method that takes an object as a parameter<br>
    public static void printBookTitle(Book book) {<br>
        System.out.println(book.title);<br>
    }


  Wrapper Classes
  -----------------------------
  - wrapper classes provide a way to use primitive data types (like int, boolean, etc.) as objects. They are useful for situations where you need an object instead of a primitive type, such as in collections like ArrayList, which can only store objects.
  - eg.,  Integer integerObject = Integer.valueOf(10); // Boxing/Object <br>
        int primitiveInt = integerObject.intValue(); // Unboxing

  Records
  ----------------------------
  - Records provide a concise way to create immutable data classes that automatically provide implementations for common methods like equals(), hashCode(), and toString().
  - eg., public record Person(String name, int age) { <br>
}

Inheritance
------------------------------
- Inheritance is like when a new class takes on all the stuff from another class, becoming an extension of it.
- Inheritance allows one class (subclass) to inherit fields and methods from another class (superclass), enabling code reuse.
- eg.,<pre> // Superclass <br>
class Animal { <br>
    void eat() { <br>
        System.out.println("This animal eats food."); <br>
    }<br>
}<br></pre>
<br>
<pre>// Subclass<br>
class Dog extends Animal {<br>
    void bark() {<br>
        System.out.println("The dog barks.");<br>
    }<br>
} <br>
<br></pre>
<pre>// Main class to test inheritance<br>
public class Main {<br>
    public static void main(String[] args) {<br>
        Dog dog = new Dog();<br>
        dog.eat(); // Inherited method<br>
        dog.bark(); // Subclass method<br>
    }<br>
}<br>
<br></pre>

Sealed Classes
------------------------------
- Sealed classes in Java provide a way to restrict which classes can extend or implement them.
- This feature was introduced to improve control over inheritance and ensure a more predictable and maintainable class hierarchy.
- By using sealed classes, you can explicitly specify a limited set of permitted subclasses.
