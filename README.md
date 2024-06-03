# JAVA
Java is a widely-used programming language that acts as a bridge for humans to communicate with computers. It's especially popular among beginners because it's relatively straightforward to learn and use.
# What Can Java Do?
Software engineers use Java to create a variety of applications, including:
- **Web applications**: Programs that run on web servers and are accessed through browsers.
- **Mobile applications**: Apps for smartphones and tablets.
- **Desktop applications**: Programs that run directly on personal computers.
# Running Java Programs
To run Java programs, your computer needs a special software component called the Java Runtime Environment (JRE). The JRE allows Java programs to work on your computer by providing the necessary resources.
# Writing Java Programs
To write and compile (turn into a format the computer can execute) Java programs, you need the Java Development Kit (JDK). The JDK includes:
- The JRE
- Compilers (tools to convert your Java code into a runnable program)
- Additional tools to help you develop Java applications

When you install the JDK, you automatically get the JRE along with it, making it easy to write and run Java programs.
# Visual Explanation
1. **Writing Code**: You write Java code using a text editor or an Integrated Development Environment (IDE).
2. **Compiling Code**: You use the JDK to compile your code, transforming it into a format the computer understands.
3. **Running Programs**: You use the JRE to run the compiled program on your computer.
This whole process allows you to create functional software that can perform a wide range of tasks, from simple calculations to complex web services.

# Algorithms in Programming
Computers are a part of our daily lives, whether at work, home, or on the move. However, they aren't smart on their own; they are simply data processors. To perform any task, they need precise instructions, known as a program.
Initially, these instructions were written in binary code (zeros and ones), the only language computers understand. Fortunately, programmers developed higher-level languages like Java, which are easier for humans to write. These languages are then translated into binary code for the computer.
Algorithms are essential in programming. They are step-by-step guides that computers follow to solve problems. When a problem arises, an algorithm combined with a programming language can provide a solution.
This algorithm can then be implemented using a programming language like Java to work in real life.

# Java Essentials
# Packages
In Java, a package is like a folder that contains Java files. To create a package in IntelliJ, follow these steps:

1. **Start a New Project**: 
   - Open IntelliJ and select 'New Project.'
   - Choose Java and click 'Next.'
   - Do not select a template.
   - Name the project (e.g., "Fundamental") and click 'Finish.'

2. **Project View**:
   - On the left, you'll see the project view where all your files are stored. Since the project is new, it will be empty.

3. **Source Code**:
   - 'Source code' refers to the computer programs you write.

4. **Create a New Package**:
   - Right-click the source folder.
   - Select 'New' and then 'Package.'
   - Name the package (use lowercase letters as a common practice). For this example, name it 'gross_calculator.'

5. **Naming Conventions**:
   - Using lowercase letters for package names is a widely followed convention in Java programming.
By following these steps, you'll see the new package 'gross_calculator' in the project view, ready to hold related Java files. Great job on creating your first package!


# Classes
To create a new class in Java, follow these steps:

1. **Create a New Class**:
   - Right-click on the package.
   - Select "New" and then "Java Class."
   - Name the class, typically starting with an uppercase letter. For example, name it "GrossPayCalculator" (using CamelCase without spaces).

2. **Naming Conventions**:
   - Java class names should follow the convention of starting each word with an uppercase letter.

3. **Class Creation**:
   - After naming the class and pressing 'Enter,' the class will be created in the package.

4. **Java File Structure**:
   - Java files have a ".java" extension.
   - The first line in the Java file should declare the package name if the file belongs to a package, using the format: `package packageName;`.

5. **Class Declaration**:
   - After the package declaration, declare the class using: `public class ClassName { }`.

Example for "GrossPayCalculator":
```java
package gross_calculator;

public class GrossPayCalculator {
    // Code for the class goes here
}
```


# Main Method
In Java, the code within curly braces `{}` is part of a class or method. Here's how to create and run a main method, which is where a Java program starts executing:

1. **Creating the Main Method**:
   - Inside your class, write the main method as:
     ```java
     public static void main(String[] args) {
         // Code goes here
     }
     ```
   - This method is essential for running the program. Java looks for this method to start execution.

2. **Adding a Print Statement**:
   - To display something on the console, use:
     ```java
     System.out.println("Hello, World!");
     ```
   - This line tells Java to print "Hello, World!" to the console. The semicolon `;` marks the end of the instruction.

3. **Running the Program**:
   - Save your file.
   - Right-click anywhere in the program and select 'Run.'
   - The console window will open and display "Hello, World!"
  
# Reserved Words
In Java, certain words are reserved and have special meanings defined by the language, such as "package," "public," "class," "static," and "void." These words are highlighted in different colors in your code editor.
# Key Points:
- **Reserved Words**: These are special terms with specific purposes in Java.
- **Naming Restrictions**: You cannot use reserved words to name variables or other elements in your program.
- **Highlighting**: In your code editor, reserved words are often highlighted in different colors to indicate their special status.

Keep an eye on the color changes in your code to recognize reserved words.


# Java Variables
# Creating Variables
To calculate an employee's gross pay, follow these steps in the main method:

1. **Comments**: Use comments to leave notes in your code. Comments start with `//` and are ignored by the computer.

2. **Defining Variables**:
   - **Hours Worked**: Create a variable to store the number of hours worked.
     ```java
     int hours = 40;
     ```
     - `int` is used for integer values.

   - **Pay Rate**: Create a variable to store the hourly pay rate.
     ```java
     double payRate = 25.50;
     ```
     - `double` is used for decimal values.

3. **Calculating Gross Pay**:
   - Multiply hours by pay rate and store the result in a new variable.
     ```java
     double grossPay = hours * payRate;
     ```

4. **Printing the Result**:
   - Use `System.out.println` to display the gross pay.
     ```java
     System.out.println("Gross Pay: " + grossPay);
     ```

5. **Running the Program**:
   - Run the program to see the result. 

# Example Code
Here’s the complete code for the gross pay calculator:

```java
public class GrossPayCalculator {
    public static void main(String[] args) {
        // Define variables
        int hours = 40;
        double payRate = 25.50;

        // Calculate gross pay
        double grossPay = hours * payRate;

        // Print the result
        System.out.println("Gross Pay: " + grossPay);
    }
}
```

# Primitive Data Types

Java has eight primitive data types:

1. **Integral Types (Whole Numbers)**:
   - **byte**: 8-bit, max value 256.
   - **short**: Larger than byte.
   - **int**: Standard for integers.
   - **long**: 64-bit, handles up to 9.2 quintillion.

2. **Decimal Types**:
   - **float**: Up to 7 decimal digits.
   - **double**: Up to 16 decimal digits, more precise.

3. **Boolean Type**:
   - **boolean**: Only `true` or `false`.

4. **Character Type**:
   - **char**: Holds a single character. Use single quotes (e.g., `'A'`).

These data types cover most basic needs in Java programming.


# Local Variable Type Inference

In Java, you can use `var` for local variables, letting Java determine the data type based on the assigned value. For example:

```java
var isWaterWet = true;
```

# Key Points:
- **Use `var`**: Instead of specifying the data type, use `var`.
- **Immediate Assignment**: You must assign a value when you declare the variable with `var`.
- **Local Variables Only**: This works only for variables declared within a method, not for class-level (global) variables.

This feature simplifies code and reduces the need for explicit type declarations for local variables.

# Naming Variables
In Java, it's crucial to use descriptive names for variables to enhance code clarity. Instead of shortcuts like 'h' for hours or 'r' for rate, opt for clear names like 'hours' and 'payRate' to make your code easily understandable.

# Guidelines for Naming Variables:
- **Descriptive Names**: Use names that clearly represent the variable's purpose.
- **Consistency**: Maintain consistent naming conventions throughout your codebase.
- **Java Naming Conventions**:
  - Start with a lowercase letter.
  - Use camel case for multiple words (first word lowercase, subsequent words uppercase).
  - Numbers are acceptable within the name but not as the first character.
  - Special characters like $ or _ are allowed, but avoid dashes.
  - Avoid Java's reserved words.
- **Compiler Assistance**: If you make naming errors, the compiler will notify you.

# Modifying Variables
In the original GrossPayCalculator program, the values for hours and pay rate were fixed, meaning they stayed the same every time the program ran. To make the program more adaptable, we can initialize these variables to zero and then prompt the user to input their values.

# Steps for Modification:
1. **Initialize Variables**:
   - Set the variables for hours and pay rate to zero initially.

2. **User Input**:
   - Use a scanner to read input from the user.
   - Import the Scanner class from the java.util package.
   - Read the user's input and store it in the hours and pay rate variables.

3. **Closing Scanner**:
   - Close the scanner object to prevent memory leaks.

By implementing these changes, the program becomes more flexible, allowing users to input different values for hours and pay rate each time it runs.

# Arithmetic Operators
In Java, there are five basic arithmetic operators for working with numeric values:

1. **Addition**: `+`
   - Adds two numeric values together.
   - Can also append a value to a string.

2. **Subtraction**: `-`
   - Subtracts one value from another.

3. **Multiplication**: `*`
   - Multiplies two values together.

4. **Division**: `/`
   - Divides one value by another.

5. **Modulo Operator**: `%`
   - Returns the remainder of dividing one value by another.

These operators are used with numeric data types like bytes, shorts, ints, longs, floats, and doubles to perform basic mathematical calculations.


# Decision Structures in Java: If Statements

In Java, we use decision structures to provide different paths for our programs to take. The most common decision structure is the "if statement."

# If Statements:
- **Function**: Think of an if statement as a side road in the program. If a certain condition occurs, the program takes that side road and executes a specific block of code, then returns to the main path of execution.
- **Example**: Suppose we have a team of salespeople earning a standard rate of \$1,000 a week. However, if any of them make more than 10 sales, they receive an extra bonus of \$250. 
- **Implementation**: We use an if statement to check if the number of sales exceeds the quota. If it does, we add a bonus of \$250 to their payment; otherwise, no bonus is added.

# Example Code:
```java
int sales = 15; // Example sales count
int standardPay = 1000; // Standard weekly pay
int bonus = 250; // Bonus amount

// Check if sales exceed the quota
if (sales > 10) {
    standardPay += bonus; // Add bonus to payment
}

System.out.println("Weekly payment: $" + standardPay); // Print the weekly payment
```

# Testing:
- **Debug Mode**: Run the code in debug mode to step through it line by line.
- **Outcome**: With 10 sales, the if statement doesn't run, and the payment remains \$1,000. With 15 sales, the if statement executes, adding a \$250 bonus, resulting in a payment of \$1,250.

  ### If-else Statements

In Java, the if-else statement is a decision structure that allows a program to choose between two paths based on whether a certain condition is met or not.

#### Function:
- **Decision Making**: With if-else, a program can take one of two paths depending on whether a condition is true or false.
- **Example**: For instance, a program can use if-else to check if a salesperson has met their quota and print a congratulatory message if they have, or print a reminder message if they haven't.

#### Example Code:
```java
int quota = 10; // Initialize quota
int sales = 8; // Example sales count

// Check if sales meet the quota
if (sales >= quota) {
    System.out.println("Congratulations! You met your quota.");
} else {
    int salesShort = quota - sales; // Calculate sales short
    System.out.println("You did not meet your quota. You were short by " + salesShort + " sales.");
}
```

# Explanation:
- **Initialization**: The code initializes the quota to 10.
- **Input**: It then asks the user how many sales they made this week.
- **Decision Making**: Using if-else, it checks if the sales are greater than or equal to the quota.
- **Output**: If the condition is met, it prints a congratulatory message; otherwise, it prints a message indicating how many sales were short.
  The if-else-if statement is a useful tool for directing a program's flow based on various conditions. It's handy for tasks like grading tests or deciding on discounts.

# switch statement
The switch statement is like an expanded version of the if-else-if structure, ideal for handling multiple options. While if-else-if checks conditions, switch compares for equality. For instance, if a user inputs their grade, we can use switch to display a corresponding message.

here is an example, we have a class where users input their letter grades. We want to assign a message to each grade. Here's how we do it:

1. We create a "switch" and place the user's grade inside it.
2. Inside the switch, we list different "cases" for each possible grade.
3. Each case contains the corresponding message we want to assign.
4. After each case, we add a "break" to move out of the switch.
5. If none of the cases match, we use "default" as a catch-all for unexpected inputs.

# Switch expression
Switch expressions offer a simpler way to handle tasks compared to switch statements. Instead of declaring a message separately and then assigning it, you can combine both steps with switch expressions.

Here's how it works:

1. After the message variable, add an equal sign.
2. Move the switch structure to the right side.
3. Use an arrow (a dash followed by a greater than sign) instead of ":message=". This assigns the message based on each case.
4. You can remove break statements, making the code cleaner.
5. Finish with a semicolon after the closing curly brace for a tidy look.

Switch expressions are handy when you need to run the same code for multiple cases. Just list them separated by commas. For example, if A and B grades should have the same message, add a comma after case A and specify case B as well.
Switch expressions aren't limited to assignments; you can include more than just assignments in your cases. Simply enclose all case statements in curly braces after the arrow.
When deciding between a switch statement and a switch expression, consider your needs. If you need to assign a value, go with switch expressions. If you only need to run statements, stick with switch statements.

# Relational operation
Relational operators are like tools for making decisions in Java. They help determine if something is true or false. 

Here are the six special operators:

1. Greater Than Operator (>): Checks if the number on the left is bigger than the one on the right. For example, "Is 2 greater than 3?" No, that's false.
2. Less Than Operator (<): Checks if the number on the left is smaller than the one on the right. For example, "Is 2 less than 3?" Yes, it is!
3. Greater Than or Equal Operator (>=): Checks if the number on the left is either bigger or equal to the one on the right. For example, "Is 4 greater than or equal to 4?" Yes, it is.
4. Less Than or Equal Operator (<=): Checks if the number on the left is either smaller or equal to the one on the right. For example, "Is 4 less than or equal to 3?" No, it's false.
5. Equal To Operator (==): Checks if two things are equal. In Java, you use a double equal sign (==). For example, "Is 3 equal to 2?" No, it's false.
6. Not Equal To Operator (!=): Checks if two things are not equal. In Java, you use an exclamation mark and an equal sign (!=). For example, "Is 3 not equal to 2?" Yes, it is not equal.

 ***Remember, these operators work with most data types except booleans. You can't use them with booleans.***

 # Logical Operators
 Logical operators in Java help you combine conditions to get a clear yes or no answer. They're useful for making complex decisions. Here's a breakdown:

1. AND (&&): Combines two conditions, and both must be true for the overall result to be true.
2. OR (||): Looks for at least one condition to be true to get a true result.
3. NOT (!): Flips the truth of a single condition. If the condition is false, NOT turns it into true.

For example:

- AND Operator: If "one <= two" is true AND "four != five" is true, the result is true.
- OR Operator: If "three == four" is false OR "six > one" is true, the result is true.
- NOT Operator: If "two != three" is false, applying NOT makes it true.

These operators are useful for combining conditions in if-else situations, like determining loan eligibility based on salary and job tenure. With logical operators, you can keep your code clean and avoid nested if statements.

# Short circuit logic
Short Circuit Logic is a way to speed up logical operations by stopping evaluation when the outcome is already known. 

With 'and', if the first condition is false, there's no need to check the second because both must be true for the whole expression to be true. Similarly, with 'or', if the first condition is true, there's no need to check the second because just one true condition is enough for the whole expression to be true.

In an example with three conditions, the program checks them in order. If the first combination yields false, it doesn't check the rest because the final outcome can't be true. If the first condition yields true with 'or', the program doesn't check the second. With 'and', if the first condition is true, it still checks the second because both need to be true for the whole expression to be true.

Understanding short-circuiting can help optimize condition organization.

# Repetition structure
Repetition Structures in Java, like the While Loop, are like magic spells for code, making it repeat tasks effortlessly. Instead of copying and pasting code repeatedly, loops streamline the process by executing the same instructions multiple times.

Imagine managing a store where each employee earns $15 per hour. Now, here's the challenge: you want a program to calculate their weekly pay without allowing any overtime. The program, let's call it "GrossPayInputValidator," asks for weekly hours worked and calculates gross pay, but it ensures no overtime by limiting hours to 40 per week.

To ensure valid input, we employ a loop. Using the "while" keyword and a condition in parentheses, we create a loop. If the condition holds true, the loop executes the code inside the curly braces.

The loop triggers if the input exceeds the maximum hours allowed. Inside, an error message alerts the user and prompts for correct input. The loop repeats until valid input is received, indicated by the condition becoming false, allowing the program to proceed.

Testing the program with inputs over 40 hours prompts error messages, while inputs under 40 exit the loop, displaying the calculated pay.

Remember, if a loop's condition depends on a variable, ensure the variable can change within the loop to avoid infinite loops, which endlessly run until the program crashes.

While loops are ideal for scenarios where code execution depends on a condition remaining true. They check the condition before each iteration, ensuring efficient execution based on dynamic conditions.

# Do while loop
The Do While Loop is similar to the While Loop but with a twist—it checks the condition after running once, ensuring at least one execution. Although less commonly used than the regular While Loop, understanding how it operates is valuable.

Consider a program that continuously performs calculations based on user input until they opt out. Using a Do While Loop, the program initiates with a "do" followed by braces containing the loop's actions. Then, a "while" statement with a condition inside parentheses, ending with a semicolon.

In this scenario, the condition revolves around the user's desire to continue. We set a variable, "runAgain," starting at zero. If "runAgain" equals one, the loop repeats. Within the loop, we interact with the user, collect numbers, perform calculations, and display results.

Updating "runAgain" ensures the loop's continuation or termination based on user input. If the user chooses to continue ("1"), "runAgain" updates accordingly; if they opt out ("2"), the loop ends.

Executing the program triggers the Do While Loop, allowing user input and calculations. Even if just once, the loop executes before user input determines its fate.

The key distinction of the Do While Loop is its execution at least once, making it suitable for situations where an initial operation is essential, followed by potential repetitions based on a condition.

# For loop
The For Loop stands out among other loops because it's all about counting. Picture a cashier scanning items, and the for loop helps tally the total cost by keeping track of the count.

To set up a for loop, we first define a counter, usually named "i," to track the loop's iterations. Then, we specify a condition to determine when the loop stops—typically, this condition compares the counter to the desired number of iterations. Finally, we update the counter within the loop to ensure the loop progresses.

Inside the loop, we prompt for item prices and add them to the total. Once the loop completes its iterations, we print the total cost.

Running the program in debug mode allows us to track the loop's progress, observing how the counter and total change with each iteration.

Key factors to remember about for loops: they're about counting and adhere strictly to the specified number of iterations. They also check the condition before executing, making them reliable for situations where the number of repetitions is known in advance.

# Nested loop
Nested loops are like Russian nesting dolls, where one task contains smaller repetitive tasks within. Take, for instance, calculating the average test scores for a class of 24 students, each taking four tests.

Using for loops, we first loop through each student. Setting a variable, "i," to start at zero and incrementing it until it reaches the total number of students, ensures we focus on one student at a time.

Within this loop, we delve into each student's test scores, which calls for another loop since there are four tests per student. To avoid confusion with the outer loop's counter, we introduce a new variable, "j," starting at zero and running for the four tests.

Before diving into the inner loop, we initialize a "total" variable to zero to accumulate the test scores. Inside the inner loop, we prompt for each test score and add it to the total. To maintain clarity, we display the test number as "j + 1" and read the score into a variable called "score."

Exiting the inner loop, we calculate the average test score for the student by dividing the total by the number of tests and print it out, ensuring the student number is displayed as "i + 1" for clarity. This process repeats for all 24 students, computing the average of their four test scores.

Remember, this example illustrates nested for loops, but you can nest different loop types depending on the specific task at hand, be it while loops within while loops or a combination of while and for loops.

# Break Statement
The break statement is your ticket out of a loop when you need to escape, no questions asked. Picture hunting for the letter 'A' in a string using a For Loop.
We set up the loop, starting at zero and running until the end of the text. Inside, we grab each letter and store it in 'currentLetter.' If 'currentLetter' is 'A' (uppercase or lowercase), we signal success by setting 'letterFound' to true. Then, we break out of the loop right away using the 'break' keyword, regardless of what's left to do in the loop. Simple as that!

# Methods In Java
In Java, methods are like specialized tools in a toolbox within a class. They break big problems into smaller, manageable tasks and prevent code repetition. While they may be called functions or modules in other languages, in Java, they're known as methods.

Consider the main method, a staple in every program, alongside others like those in the scanner class for input and system class for output.

A method's job is to perform calculations and provide an answer. Let's dissect its structure. The header, akin to an ID card, indicates who can use it, with "public" meaning it's accessible to all. It also includes non-access modifiers like "static" or "final," and specifies the return type, indicating the type of answer the method will provide, such as "int" for a whole number.

Methods can only return one thing. Next, the method's name, starting with a verb and possibly a descriptive word or two, followed by parentheses, acting as a mailbox for required information. Every method has a signature, which comprises its name and the information it needs in the parentheses, distinguishing it from others.

After the header, the body, enclosed in curly braces, contains the actual code executed when the method is called. If the method isn't void (meaning it returns something), it must include a return statement at the end to provide the answer.

Understanding a method's structure helps in effectively utilizing them in Java programming.

# Calling Methods
In Java, methods need a gentle push to start working. Let's say we're building a program and creating a method to greet users by their names. After defining this method, we need to activate it from our main method.

The order in which methods are written within a class doesn't affect their behavior; what matters is the order in which they're called. Even if our greetUser method is placed after the main method, it could be at the beginning—it wouldn't change how it works.

Now, here's the deal: the greetUser method asks for the user's name, stores it, and then gives a friendly greeting. But simply writing the method won't make it do its thing. Methods aren't psychic; you need to summon them by name.

When you start a Java program, it begins in the main method automatically—no need to call it. So, that's where we begin. To activate the greetUser method, you simply type its name followed by empty parentheses and a semicolon wherever you want it to run. This small command wakes up the greetUser method, making it ready to greet users when the class is fired up. Easy, right?


# Vriable Scope
In programming, methods wait for a signal before they start. Let's say we're writing code to greet someone by name and then calling this method from our main code. All methods must hang out within a class, but their order doesn't matter much.

Now, about variables—they're like unique stickers, only usable where they're born. If you declare a variable inside curly braces (like method1), you can only use it there. Mentioning it elsewhere, like in method2, will cause an error because the variable belongs to method1's space.

The scope of a variable isn't just limited to methods; it can be even narrower, like within a specific block of code. For example, a variable named "myVariable" defined within an "if" structure can only be used within that block.

Local variables are defined within methods, like those inside loops or decision structures. Global variables, declared outside methods, have a broader reach, extending throughout the class.

You can have variables with the same name in different scopes. When referencing a variable, the narrower-scoped one takes precedence. For instance, if a global and a local variable share a name, the local one is used within its scope. To explicitly refer to the global variable from a local scope, you can use the "this" keyword.

When deciding between global and local variables, consider where you'll need to use them. Use local variables for limited use, and global ones for broader accessibility across multiple methods.

# Passing Data To Methods
Methods often require external data to do their job. They receive this data through parameters. Picture creating a method to determine if someone qualifies for a loan based on salary and credit score. In our main method, we collect the user's salary and credit score. Now, we need a method, "isUserQualified," to make the decision.

This "isUserQualified" method needs access to the user's salary and credit score. Since these variables are stuck inside the main method, we include them as parameters in the "isUserQualified" method. Each parameter gets a data type and name, like "int_creditScore" and "double_salary."

Inside "isUserQualified," we introduce two more variables: one for the required salary ($25,000) and another for the required credit score (700). Then, we use an "if" statement to check if the user meets these conditions and print an approval or decline message accordingly.

To make our method work, we call it from the main method, passing in the credit score and salary as arguments. Even if the variable names differ in the main method and "isUserQualified," there's no confusion because they exist in different scopes.

Switching variable names in the main method doesn't cause errors as long as we update the method call accordingly. The order of arguments must match the parameter list's order, ensuring clarity for the compiler.

# Returning Data From Methods
Methods can do things and sometimes give back results. Take the "isUserQualified" method, for example. Initially, it only did its job without giving anything back, like a one-way street. But now, we want it to return a yes or no, like thumbs up or thumbs down. So, we change its return type to boolean. If everything checks out inside the "if" statement, it returns true; otherwise, it's false.

Now, when we use a method that returns something, we can catch that result and store it in a variable. Remember when we did that with the "next double" method? This time, we do the same with "isUserQualified" and call it "qualified."

Next, look at the "notifyUser" method. It needs a yes or no (a boolean) when we call it. Inside, it decides what message to give us based on the yes or no. So, when we call it from the main method, we pass it the "qualified" variable.

When we run the program, the "qualified" variable gets its answer from "isUserQualified." If it's false, "notifyUser" says, "Sorry, you have been declined." It's like following a flowchart.

# Overloading Methods
In a class, you can have multiple methods with the same name but different features, which is called overloading. In our "month" class, for example, there are two "getMonth" methods. A method's signature includes its name and parameter list. One method takes an integer for the month, while the other takes a string. You can overload as many methods as you need, as long as their parameter lists are different.

When you call an overloaded method, the compiler identifies which one you mean by matching the argument to the method's parameter list. If you try to create overloaded methods with the same parameter list, you'll get a compilation error saying the method is already defined. Even if you change the argument name, it won't work if the parameter list is identical.

Overloading methods is useful for offering similar methods with slight differences. It keeps your code tidy by avoiding complex conditional logic in a single method.

# Objects In Java
Objects in programming are like containers holding both data and actions. By creating an object, you can utilize its data and actions throughout your code. Picture it as crafting a blueprint for a rectangle, detailing all its features.

Now, let's think about a rectangle as more than just a concept; envision it as something tangible, like an object you can hold. It possesses characteristics, such as length and width, akin to its ID tags. We term these identifiers "fields." For instance, you might declare these fields as "double length" and "double width."

But what can we do with this rectangle? Well, we can measure its sides and compute attributes like its perimeter and area. These measuring actions are termed "methods." For instance, you might define methods like "double calculatePerimeter" and "double calculateArea," where you return mathematical computations based on the rectangle's dimensions.

However, keep in mind that this class isn't designed to perform actions by itself; it's merely a blueprint for creating rectangle objects. If you desire a specific rectangle, you'll need to provide it with values for length and width later on.

At present, the rectangle has no assigned values. Attempting to calculate its perimeter is akin to computing the area of thin air. To remedy this, we implement "getter" and "setter" methods. These methods enable you to retrieve or update the length and width values as needed.

In the realm of classes, there's a concept called encapsulation, a foundational principle in object-oriented programming (OOP). Encapsulation stipulates that a class's data (its fields) should be kept private, while its methods (defining its behavior) can be shared with other classes. To adhere to encapsulation, we designate our length and width fields as "private" and mark the methods we wish to share as "public."

Furthermore, there's another access modifier called "protected," serving as a semi-public VIP area accessible only to classes within the same package. As for the class we're constructing here, it's akin to the blueprint for a rectangle.

# Java Constractors
Java constructors are a way to assign initial values or configure the state of an object. Every object has a constructor, and the default one, encountered first, is known as the default constructor.

This default constructor doesn't take any parameters, so if you're not ready to decide on a rectangle's length or width yet, you can use it without providing any values. In Java, even if you don't explicitly define a default constructor, one is still there, working quietly in the background as an empty constructor.

Let's dissect this constructor. It starts with a keyword like 'public' and doesn't have a return type, resembling methods. Then, its name matches the class name exactly, in this case, 'rectangle'. There could be parameters in the parentheses, but in our default constructor, there are none. Finally, there are curly braces for the body.

The aim of this default constructor is to assign default values to the class's fields, such as setting the length and width to zero.

You can have multiple constructors with the same class name but accepting different parameters. For example, let's create another constructor for those who know the length and width upfront. Again named 'public Rectangle', this time it takes 'double length' and 'double width' as parameters. To set these fields, we call the setter methods and pass in the received parameters. This gives us options for setting up a rectangle's state with different constructors.

# Object Instantiation
To create objects in Java, like rooms using the Rectangle class, you start by specifying the object's data type, which is the class it's based on. For our rooms, that's Rectangle. Give the object a name, like "room1", and then create an instance using the keyword "new" followed by the class's constructor. We'll stick with the default constructor here, so it's simply "Rectangle()".

Once the object is created, you can access its methods using the dot operator. For example, you can set the room's width and length with "setWidth" and "setLength", and then calculate the area with "calculateArea".

You can also create another room object using a constructor that takes the length and width as arguments, like "Rectangle room2 = new Rectangle(30, 75)". This assigns the given values to the length and width directly.

The Rectangle class, like many others, can be used for various purposes. In our case, it serves as a blueprint for rectangles, and we're using it to model rooms in a house. This flexibility is one of the strengths of classes in Java, allowing you to create specific objects tailored to your needs.

# Method Parameters as Objects
You can use objects as method arguments just like primitive data types. For example, if you have two Rectangle objects representing rooms, like the kitchen and bathroom, you can calculate their total area.

To do this, you create a method called calculateTotalArea. It returns a double and takes two Rectangle objects as input. Inside the method, you use the dot operator to call their calculateArea methods and return the sum.

In the main method, you call calculateTotalArea with the kitchen and bathroom objects as arguments. Finally, you print the total area with a message like "The total area is" followed by the area value. This is how you use objects as method parameters.

# Methods Return Type
To get both the length and width of a rectangle, we can create a method that returns an object containing these dimensions.

Instead of directly assigning fixed values to the kitchen and bathroom objects, we'll use a method called getRoom. This method will prompt the user for the dimensions and return a Rectangle object with those values.

In the getRoom method, we specify the return type as Rectangle. After obtaining the length and width, we create a Rectangle object using that information and return it using return new Rectangle.

It's important to note that we're not storing this new object within a variable inside the getRoom method. Instead, we pass it directly to the room objects in the main method.

For example, for the kitchen, we'll set the length as 200 and the width as 400. Similarly, for the bathroom, the length is 300 and the width is...

# Wrapper Classes
Wrapper classes are like magic wands for primitive data types. Let's take two friends: number1 (an int) and number2 (an Integer, which is the fancier version of int). Number2 becomes an object thanks to this transformation. The beauty of wrapper classes is their collection of handy methods.

These wrappers cover all basic data types. Let's focus on the Integer wrapper class. It's a treasure trove for handling integers. There's MIN_VALUE and MAX_VALUE for the smallest and largest integer values, compare and compareTo methods for comparing integers, conversion tricks like doubleValue and floatValue to switch integers to other data types, and the super-handy parseInt method that magically transforms number strings into actual integers.

If you ever need to convert a plain integer variable into an Integer object to use these methods, you can use the valueOf method. Similar tricks exist in other wrapper classes too.

For more details, don't forget to check out the Java docs!

# Records
Records are like simplified versions of Java classes, perfect for handling simple objects with fields and methods. Let's say you want to create an "account" model. Instead of using "class", you use "record" and list your fields within parentheses and curly braces. Voilà! You have a record with those fields. No need to worry about creating getter or setter methods; they're automatically generated in the background. But if you want more methods, just add them inside those curly braces.

Creating records is as easy as creating classes. For our "account" example, you'd simply say "new account" and provide all the values through the constructor. Records are immutable, meaning once you set the field values, they can't be changed. While records don't have setter methods, they do have accessor methods. These methods bear the same name as the field itself, like "account.balance" instead of "account.getBalance".

Records are fantastic for managing simple objects that you set up once and access later in your code. They're often referred to as POJOs, or Plain Old Java Objects. In essence, records offer a streamlined way to simplify code for basic objects.

#  Inheritance Simplified

**Inheritance Overview**

Inheritance allows a new class to adopt the properties and methods of another class, effectively extending it. 

**Key Players in Inheritance:**
- **Parent Class (Superclass, Base Class)**: The class that passes on its attributes and methods.
- **Child Class (Subclass, Derived Class)**: The class that inherits from the parent class.

**How It Works:**
Subclasses are specialized versions of their superclasses, inheriting and extending their functionality.

**Example: Person and Employee Classes**

- **Person Class**: Contains attributes like `name`, `age`, and `gender` with corresponding getter and setter methods.
- **Employee Class**: Inherits from `Person`, adding attributes like `employeeId` and `title`.

Using the `extends` keyword, the `Employee` class inherits all properties and methods from `Person`, allowing it to add unique attributes without redefining inherited ones.

**Constructors in Inheritance**

When creating an instance of a subclass:
1. The superclass constructor is called first.
2. The subclass constructor runs next.

To explicitly call a different superclass constructor, use the `super` keyword with the required parameters. This call must be the first statement in the subclass constructor.

**Overriding and Overloading Methods**

- **Overriding**: A subclass can provide a specific implementation for a method already defined in its superclass. Use the `@Override` annotation to indicate this.
- **Overloading**: Methods in the same class share the same name but differ in parameter lists.

**Chain of Inheritance**

A class can inherit from one superclass, which in turn can inherit from another class, creating an inheritance chain. For example:
- **Vehicle Class**: Attributes like `color` and `mileage`.
- **Car Class**: Inherits from `Vehicle`, adds `doors`.
- **Coupe Class**: Inherits from `Car`, specifies `doors` as 2.

Creating an instance of `Coupe` allows it to use methods and properties from `Vehicle` and `Car`, illustrating the chain of inheritance.
Inheritance in Java allows for efficient code reuse and organization through class hierarchies. Superclass constructors run before subclass constructors, and method overriding and overloading provide flexibility in how inherited methods are implemented and used. This chain of inheritance supports a structured and hierarchical approach to object-oriented programming.

### Limiting Access in Inheritance

**What Subclasses Inherit:**
- **Public and Protected Members**: These are inherited by the subclass.
- **Private Members**: These are not inherited and remain exclusive to the superclass.
- **Final Methods**: These are inherited but cannot be modified by the subclass.

**Access Modifiers and Inheritance:**

- **Protected**: Members marked as protected in the superclass can be accessed by the subclass.
- **Public**: Members marked as public in the superclass are accessible to the subclass.
- **Private**: Members marked as private in the superclass cannot be accessed or inherited by the subclass.

**Example: Using Protected Fields**

In the `Square` class, fields like `side` and `length` from the `Rectangle` class are accessible because they are protected. If `side` were private, it would not be accessible in the `Square` class, leading to an error.

**Overriding Methods and Access Modifiers:**

- When overriding a method, the access level cannot be more restrictive than the original method.
- For example, if the `calculatePerimeter` method in `Rectangle` is public, the overridden method in `Square` must also be public or can be less restrictive, like protected. All i can say is that
In Java inheritance:
- Constructors are not inherited.
- Public and protected members are inherited, but private members are not.
- Final methods are inherited but cannot be modified.
- Access modifiers control what can be shared and overridden between superclasses and subclasses.

# Sealed Classes

**What Are Sealed Classes?**

Sealed classes in Java restrict which other classes can inherit from them. They allow specific classes to inherit while blocking others.

**How to Create a Sealed Class:**
- Use the `sealed` keyword in the class declaration.
- Specify permitted subclasses using the `permits` clause.

**Example: Shape Class**

```java
public sealed class Shape permits Circle, Rectangle {
    // class content
}
```

In this example, only `Circle` and `Rectangle` can inherit from `Shape`.

**Rules for Subclasses of Sealed Classes:**
- **Sealed**: Follows the same inheritance restrictions as the parent sealed class.
- **Non-sealed**: Allows any class to extend it.
- **Final**: Cannot be inherited by any other class.

**Example: Subclass Declarations**

- **Sealed Subclass**:
  ```java
  public sealed class Rectangle extends Shape permits Square {
      // class content
  }
  ```

- **Non-sealed Subclass**:
  ```java
  public non-sealed class Circle extends Shape {
      // class content
  }
  ```

- **Final Subclass**:
  ```java
  public final class Square extends Rectangle {
      // class content
  }
  ```


- **Sealed Class**: Restricts inheritance to specified subclasses.
- **Sealed Subclass**: Inherits the same restrictions.
- **Non-sealed Subclass**: Open to any class for inheritance.
- **Final Subclass**: Closed to further inheritance.

# Polymorphism

**Polymorphism in Object-Oriented Programming**

Polymorphism is like the ability of classes to take on many forms. It allows a subclass to be treated as an instance of its superclass.

**Example with Animals, Dogs, and Cats:**

- **Superclass**: `Animal`
- **Subclasses**: `Dog` and `Cat`

**Scenario:**

- **Dog Class**: Has a method `makeSound()` that returns "woof" and a method `fetch()`.
- **Cat Class**: Has a method `makeSound()` that returns "meow" and a method `scratch()`.

**Example Objects:**
- **Rocky**: A `Dog` object. Rocky can `fetch()` and `bark()` with "woof".
- **Sasha**: An `Animal` object, but also a `Dog` or `Cat` depending on its current state.

**Polymorphism in Action:**

- When Sasha is a `Dog`, `makeSound()` will return "woof".
- When Sasha is a `Cat`, `makeSound()` will return "meow".

This illustrates polymorphism: the ability for Sasha to act as either a `Dog` or a `Cat` because both are subclasses of `Animal`.

Polymorphism allows an object to take on different forms. It enables a superclass reference to point to subclass objects, enabling dynamic method overriding. Sasha can sound like a dog or a cat, showcasing the flexibility and power of polymorphism in Java.

# Object Type Casting

**What is Object Type Casting?**
Type casting in Java involves converting an object from one type to another. This is common when dealing with polymorphism.

**Types of Casting:**
- **Implicit Upcasting**: Automatically converting a subclass object to a superclass type.
- **Explicit Downcasting**: Converting a superclass object back to a subclass type.

**Example with Animals, Dogs, and Cats:**

1. **Implicit Upcasting:**
   ```java
   Animal myDog = new Dog();
   ```
   - Here, `myDog` is of type `Animal`, but it is actually a `Dog` object. As an `Animal`, it cannot perform `Dog`-specific actions like fetching.

2. **Explicit Downcasting:**
   ```java
   Dog realDog = (Dog) myDog;
   ```
   - To access `Dog`-specific methods, we downcast `myDog` back to `Dog`.

**Practical Example:**

- **Sasha the Cat**:
  ```java
  Animal sasha = new Cat();
  sasha.scratch(); // Error: Cannot find method scratch()
  ```

- **Downcasting Sasha to a Cat**:
  ```java
  ((Cat) sasha).scratch(); // Now it works!
  ```

**Important Considerations:**
- **Class Cast Exception**: If you incorrectly cast an object to a type it is not, a runtime error occurs.
  ```java
  Dog wrongDog = (Dog) sasha; // Throws ClassCastException at runtime
  ```

- Use **upcasting** to treat a subclass object as a superclass.
- Use **downcasting** to revert back to the subclass and access specific methods.
- Ensure casts are valid to avoid runtime exceptions.

# Instanceof Operator

**What is the `instanceof` Operator?**

The `instanceof` operator in Java checks if an object belongs to a specific class or subclass.

**Example with Animals, Dogs, and Cats:**

- **Superclass**: `Animal`
- **Subclasses**: `Dog` and `Cat`

**Scenario:**

- **Object**: Sasha, an `Animal` that is actually a `Dog`.

**Usage:**

1. **Check if Sasha is an Animal:**
   ```java
   if (sasha instanceof Animal) {
       // True, Sasha is an Animal
   }
   ```

2. **Check if Sasha is a Dog:**
   ```java
   if (sasha instanceof Dog) {
       // True, Sasha is a Dog
   }
   ```

3. **Check if Sasha is a Cat:**
   ```java
   if (sasha instanceof Cat) {
       // False, Sasha is not a Cat
   }
   ```

**Practical Example: Feeding Animals:**

- **Method to Feed Animals:**
  ```java
  void feed(Animal animal) {
      if (animal instanceof Dog) {
          // Feed dog food
      } else if (animal instanceof Cat) {
          // Feed cat food
      }
  }
  ```

- **Feeding Sasha:**
  ```java
  feed(sasha); // Determines if Sasha gets dog food or cat food
  ```

**Pattern Matching:**

- **Combined Check and Cast:**
  ```java
  if (sasha instanceof Dog sashathedog) {
      // sashathedog is now treated as a Dog
  }
  ```

- The `instanceof` operator checks if an object belongs to a specific class.
- It is useful for type checking and safe downcasting.
- Pattern matching with `instanceof` simplifies checking and casting in one step.

# Abstraction: Abstract Classes and Methods

**What is Abstraction?**

In Java, abstraction is like having a rough idea or concept that isn't fully fleshed out yet. It's represented by "abstract" classes and methods, acting as templates rather than direct implementations.

**Abstract Classes:**

- An abstract class is like a blueprint, providing a general structure but not meant for direct use.
- It sets the rules and expectations for subclasses to follow.
- Abstract classes cannot be instantiated; they serve as a foundation for more specific classes.
  
**Abstract Methods:**

- Abstract methods are even more abstract; they have a name and return type but no implementation.
- Subclasses are required to provide implementations for abstract methods.
- Abstract methods are declared with the keyword "abstract" and lack method bodies.

**Creating Abstract Classes and Methods:**

- To create an abstract method, use the "abstract" keyword followed by the return type and method name, without curly braces.
- If a class has at least one abstract method, it must be declared abstract as well.

**Example: Area of Shapes**

- Define an abstract class `Shape` with an abstract method `calculateArea()`.
- Subclasses like `Circle` and `Rectangle` implement their own versions of `calculateArea()`.

Abstraction in Java allows you to create generic structures (abstract classes) and placeholder methods (abstract methods) that guide the implementation of more specific classes. It's a way to establish rules and expectations while leaving room for customization in subclasses.


# Inheriting From Abstract Classes

**Understanding Abstract Classes:**

An abstract class serves as a blueprint for other classes. When a class extends an abstract class, it inherits its structure and responsibilities.

**Example with Rectangle and Shape:**

- **Scenario**: The `Rectangle` class extends the abstract class `Shape`.

**Inheriting Abstract Methods:**

- When `Rectangle` extends `Shape`, it must either implement the abstract method `calculateArea()` or declare itself as abstract.
- If `Rectangle` doesn't implement all abstract methods, it must be declared abstract too.

**Implementation of Abstract Methods:**

- To implement an inherited abstract method, add it to the subclass and provide a concrete implementation.
- In IDEs like IntelliJ, you can use the "generate" feature to automatically implement inherited abstract methods.

**Example: Calculating Area for Rectangle:**

- **Default Implementation**: IntelliJ may provide a default implementation, but it's important to customize it.
- **Custom Implementation**: For a `Rectangle`, the area is calculated by multiplying its length and width.

Inheriting from abstract classes involves implementing or declaring abstract methods in the subclass. It's like passing on responsibilities from the abstract class to its subclasses, ensuring they fulfill their specific roles. With proper implementation, subclasses extend the functionality of the abstract class.


# Creating Objects With Abstract Types

**Understanding Abstract Classes:**

Abstract classes serve as templates and cannot be directly instantiated. They provide a blueprint for subclasses to implement.

**Example with Shape and Rectangle:**

- **Scenario**: `Shape` is an abstract class, and we want to create a `Rectangle` object.

**Using Abstract Classes as Types:**

- We cannot create a `Shape` object directly because it's abstract.
- Instead, we create instances of non-abstract subclasses like `Rectangle`.

**Example: Calculating Area of Rectangle:**

1. **Creating Rectangle Object:**
   - Instantiate a `Rectangle` object with length and width.

2. **Calculating Area:**
   - Invoke `calculateArea()` method on the `Rectangle` object.
   - Even though `Rectangle` inherits `calculateArea()` from `Shape`, its customized method is used.


- Abstract classes cannot be instantiated directly; they are templates for subclasses.
- To use an abstract class, create instances of its non-abstract subclasses.
- Subclasses must implement abstract methods or be marked as abstract themselves.
- Understanding and revisiting abstract concepts is a normal part of the learning process.

# Creating an Interface

**Understanding Interfaces:**

Interfaces are like abstract classes but more abstract. They define a blueprint for an idea without any implementation details.

**Example with Product Interface:**

- **Scenario**: We want to create an interface for products.

**Creating an Interface:**

1. **Define Interface:**
   - Create a Java class and select 'interface' as the type.
   - Name the interface following naming rules.

2. **Adding Fields:**
   - Interfaces can't have state or constructors.
   - Declare fields, but they must be public and constant.

3. **Declaring Methods:**
   - Define methods that describe behaviors.
   - Method bodies are omitted; only method signatures are provided.

4. **Example:**
   ```java
   interface Product {
       String NAME = "Default"; // Constant field
   
       String getName(); // Getter method
   
       void setName(String name); // Setter method
   }
   ```

**Key Points:**

- Interfaces are templates for classes to implement, not extend.
- Fields in interfaces are public and constant, and they must have a value.
- Methods in interfaces have no bodies and describe behaviors.
- Interfaces are powerful tools for abstraction, polymorphism, and multiple inheritance in Java.

# Implementing Interfaces

**Understanding Interface Implementation:**

Implementing interfaces in Java is akin to signing a contract. It ensures that a class adheres to the rules specified by the interface.

**Example with Book Class and Product Interface:**

- **Scenario**: We want the `Book` class to follow the rules specified by the `Product` interface.

**Implementation Process:**

1. **Connecting Interface with Class:**
   - Unlike classes, interfaces are connected using the `implements` keyword.
   - This tells the `Book` class to adhere to the rules of the `Product` interface.

2. **Fulfilling Interface Requirements:**
   - The `Book` class must implement all methods defined in the `Product` interface.
   - Failure to do so results in a requirement to declare the class as abstract.

3. **Implementing Interface Methods:**
   - Right-click on the class and instruct Java to generate and implement the required methods.
   - Customize the methods as needed, adding any necessary data like a private name.

**Adding Unique Features to the Book Class:**

- You can enhance the `Book` class by incorporating unique attributes like author names, page numbers, and ISBNs.
- Create getter and setter methods for these attributes to ensure data encapsulation and access control.

**Implementing Multiple Interfaces:**

- While a class can inherit from only one superclass, it can implement multiple interfaces.
- Simply list the interfaces separated by commas in the class header.
- Ensure compliance with the rules of all implemented interfaces.

**Dealing with Conflicting Methods:**

- If multiple interfaces have methods with the same name and signature, providing one implementation satisfies all.
- However, conflicts arise if methods have the same name but different return types, which Java does not allow.

****

Implementing interfaces in Java involves adhering to the rules specified by the interface through method implementation. It ensures consistent behavior across classes and facilitates code organization and reuse.


# Instantiating Objects with Interface Types

**Using Interfaces for Object Creation:**

In the `Book` class, we have an associated `Product` interface. Now, let's dive into creating a practical book object. Initially, we might attempt to instantiate a "product" object, but we're met with an error message. Just like abstract classes, you can't conjure them out of thin air.

**Workaround:**

However, there's a workaround. While we can't create a product directly, we can utilize any class that implements the `Product` interface, such as the `Book` class. Let's leverage the `Book` class to instantiate our book object.

**Naming the Book:**

Now, let's give our book a name using the `setName` method from the `Book` class. For instance, we can set the name to "In the Kitchen with H+ Sport" like this: `book.setName("In the Kitchen with H+ Sport")`.

**Benefits of Using Interfaces for Object Declaration:**

Using the interface for object declaration isn't mandatory, but it's beneficial if you desire polymorphic behavior. This means your object can adapt to various forms depending on the class it interacts with.

# Default and Static Methods in Interfaces

**Introduction:**

Interfaces aren't just about abstract methods; they can also contain default and static methods, offering additional flexibility. Let's illustrate this with an example. Consider a "Product" interface for products with methods to manage the product name. Then, there's a "Book" class implementing this interface. Later, we realize all products should also have a price.

**Default Methods:**

Initially, adding price-related methods directly breaks any non-abstract class implementing the `Product` interface. To prevent this, we can designate these new methods as "default." Default methods provide a default implementation, ensuring existing classes won't break. You mark them with the "default" keyword and provide a body.

**Caution with Default Methods:**

However, default methods are accessible to all implementing classes. If you don't want a book's price to default to zero, assign a different default value, like 50. While default methods are versatile with their implementation, they're not rigid. Implementing classes can override them if necessary. If no suitable default exists, it's best to leave the method abstract to prompt implementers to define their own.

**Static Methods:**

Another variant is static methods. They resemble default methods but can't be overridden by implementing classes. You can access them solely through the interface itself since interfaces can't be instantiated.

**Key Points:**

Remember, interfaces are implemented by classes and cannot be instantiated. Any class using an interface must implement its methods or declare itself abstract. By default, interface methods are public and abstract. Alongside abstract methods, interfaces can contain default and static methods, enhancing their utility in Java programming.

# Data Structure
**Collections Framework: Organized Data Storage**

Collections are like organized containers for holding various items, called elements. In Java, they're essential for managing groups of objects efficiently.

**Types of Collections:**

Collections come in different types, each with unique rules:
- Some allow duplicates, while others don't.
- Some maintain order, while others don't care about it.

**Java's Collections Framework:**

Java's collections framework, found in the `java.util` package, offers a range of tools for handling collections. At its core is the "Collection" interface, which defines common behavior for collections. Java provides other interfaces that adhere to these rules, including Set, List, Queue, and Map.

**Collections Class:**

In addition to interfaces, Java offers a handy "collections" class. It provides useful methods like "binarySearch," "copy," "frequency," and "sort" for efficiently managing collections.

**Benefits of Collections:**

Collections are foundational in Java, allowing you to efficiently manage groups of objects in your code.

**Exploring Further:**

To delve deeper into collection techniques and explore the utility class, consult the Java documentation for comprehensive information.

# Sets
**Sets: Unique Gangs of Items**

Sets in programming are like clubs with unique members; no duplicates are allowed, and they don't care about order. But you can't create a set directly; it's more like a blueprint. Different types of sets exist, such as hash sets, linked hash sets, and tree sets, each with its own details explained in the Java documentation.

**Hash Sets:**

Imagine an empty basket. To add items, like fruits, we use the "add" option. Adding apples, bananas, and lemons results in a unique collection, removing any duplicates.

**Key Points:**
- Sets don't allow duplicates.
- They're not fussy about order; it's random.
- They work with any object type.
- Use "contains" to check if a set has a specific item.
- "Remove" lets you kick out items.
- The "of" method quickly sets up a group, but beware: once used, you can't add or remove items without causing trouble.

# List
**Lists: Your Common Programming Friends**

Lists are like your go-to pals in programming, with types like array lists, linked lists, stacks, and vectors. For detailed info, check out the Java document. Let's start with an array list named "fruits".

**Array List:**

Using the "add" method, we toss in an apple, lemon, banana, and orange. The list keeps them in order, so you can grab items by position using the "get" method (remember, indexing starts at zero).

To swap out items, use "set". We swap the banana for a grape at index 2. Lists are fine with duplicates; you can add as many lemons as you like.

For hunting specific items, there's "index of" for the first occurrence and "last index of" for the last. Removing items? Use "remove", but be cautious with duplicates; it removes the first one found. We remove the last lemon at index 4.

For an unchangeable list, there's "list.of". So, we have "more fruit" and add a cherry, cranberry, and plum all at once.

# Queues
Queues: Like Waiting in Line

A queue is like standing in line at a store. You add things to it, and the first thing you added is the first to come out. You can choose from different types like linked lists or priority queues. Check out the Java documents for more info.

Using a Linked List:

Besides adding and removing, queues have special features. Items stay in order, just like in a line. You can add the same thing more than once if needed.

Following the "first in, first out" rule, when you remove something, it's the first one's turn. You can save the removed item and print it out. For example, when we removed an apple, it said so because it was at the front.

The first item in the queue is called the head. Removing it makes the next item the head. The last item is the tail.

If you want to check who's at the front without removing them from the line, use the peek method. It lets you see without making them move.


# Maps
**Maps: Like a Dictionary**

A map in Java is like a dictionary, matching keys with values. Think of a map of fruits and their calorie counts. There are different types of maps in Java, like HashMap, TreeMap, and LinkedHashMap. Here, we'll use HashMap.

**Using HashMap:**

A map isn't exactly like a collection, but it's similar. Instead of 'add', you 'put' things into a map with a key and a value. In our case, fruit names are the keys, and calories are the values, but you can use anything for keys or values.

Maps don't keep items in the order they were added, but finding something by its key is easy.

Keys must be unique, but values don't have to be.

You can update a value with 'putIfAbsent' or 'replace'.

To get something from the map, use 'get' with the key. For example, if you want to know how many calories are in a banana, you ask for 'banana'.

To remove something from the map, use 'remove' with the key.

You can check if your map has something with 'containsKey' and 'containsValue'.

For quick map creation, use 'Map.of' to make a map in one go.

# Iterators
**Iterators: Looping Through Collections**

In Java, you often need to loop through collection elements, and iterators help with that. They're provided by the collection interface.

For sets, which are unordered, there's no direct way to access items by index. But with iterators, you can still loop through them.

Here's how it works:
1. Get the iterator by calling the `iterator()` method on the collection.
2. Use a loop with the condition `iterator.hasNext()`. This checks if there are more items to process.
3. Inside the loop, print out an element using `iterator.next()`, which gives you the next element in the collection.

You can customize this loop to do whatever processing you need with the elements. Iterators work for all collections inheriting from the collection interface.

For maps, which don't inherit from the collection interface, you use the `entrySet()` method to get the map elements as a set. Then, you can use iterators to loop through them.

Iterators are a handy way to go through collection elements.

# Enhanced For Loops
**Enhanced For Loops: Looping Through Collections**

In programming, when we have a bunch of items to go through, we use enhanced for loops. They're like a special tool for looping through things.

Here's how it works:
1. Begin with `for` followed by parentheses.
2. Inside, declare the current item type and name it (e.g., `String fruit`).
3. Add a colon and the name of the collection you're looping through.
   - For example, `for each 'fruit' in the 'fruits' collection`.

Sometimes, you might get an error about types not matching. If so, be more precise when defining your collection by stating the type of elements it can contain using angle brackets.

Inside the loop, you can do whatever you want with each item. Usually, you'd process or print them. It's a straightforward way to go through collections.

Just remember, with maps, you loop through the entry set, not the map itself.

# forEach() and Lambdas
**forEach() and Lambdas: Simplifying Collection Iteration**

Using the `forEach()` method on collections makes going through them even easier than the enhanced for-loop. No need to set up a loop; just put what you want to do in the parentheses.

For example, you can use lambda expressions, which are like mini-functions. They take parameters and give results. Let's say we have a list of fruits, and we want to print each one. With lambda expressions, we write `f -> System.out.println(f)`.

If you're just calling one method, you can make it even simpler with a method reference. Instead of naming inputs and outputs, just give the class and method name, like `fruits.forEach(System.out::println)`.

The cool part? With `forEach()`, you can do more than one thing for each element. Just wrap your actions in curly braces.

Now, with Map collections, where you have both a key and a value, your lambda expression needs two inputs. You can name them anything, but `k` for key and `v` for value is common. Then you do your action, like `System.out.println(k + ':' + v)` to print the key and value with a colon in between.

In essence, `forEach()` is the modern way to go through Java collections. Practice it with your collections, and you'll find it's pretty handy.

# Functional Programming 
**Functional Interfaces in Java**

Functional programming, a style relying on mathematical functions for processing, finds its place even in Java, primarily an object-oriented language, through the `java.util.function` toolkit. Here, functional interfaces play a vital role, acting as single-job interfaces for lambda expressions and method references.

For instance, consider a list of countries. If we want to print them all, we can use `forEach` along with a lambda expression that tells it to print. This lambda expression corresponds to the `Consumer` functional interface from `java.util.function`, which has a method called `accept` that takes something and returns nothing.

To illustrate, we create a variable named `print` of type `Consumer`. When used with `forEach`, it performs the printing operation defined in the `accept` method. Even after leaving the `forEach`, we can still call the `accept` method on the `Consumer` interface and feed it data, executing our print implementation.

Besides lambda expressions, method references are also available, and there are various functional interfaces in `java.util.function`, such as:

- `Supplier`: Returns things but takes nothing.
- `Predicate`: Checks something and returns true or false.
- `Function`: Transforms one thing into another.
- Specialized operators like `UnaryOperator` and `BinaryOperator`.

These interfaces extend core interfaces and have their gang for specific operations. Additionally, they can include default and static methods. For example, the `Function` interface has a default method called `andThen`, enabling chaining of operations.

To illustrate, let's consider two operations: "Square," calculating the square of a number, and "Add," adding a number to itself. We can sequence these operations, first squaring and then adding, resulting in a final output.

While the `java.util.function` package caters to common scenarios, you can create custom functional interfaces if needed. Annotating them with `@FunctionalInterface` ensures adherence to the single-method rule, specifying input requirements and expected results. Optionally, you can include extra static or default methods for added utility.


# Streams
**Streams in Java**

Java not only provides the `java.util.function` package but also the `java.util.stream` package for functional programming needs. A stream is akin to a conveyor belt of items from a collection or array. Unlike collections, it doesn't hoard items; instead, it allows manipulation of data without altering the original source. In the `java.util.stream` package, you'll discover useful tools for these tasks.

For example, consider an array of even numbers. By converting it into a stream, we can perform operations to produce a series of odd numbers. Importantly, the original array remains unaffected.

Moreover, the stream API can operate in parallel, leveraging multiple threads to process stream items concurrently. However, this may disrupt the strict order of output, akin to a wildcard that introduces variability upon each code execution.

In essence, the stream API is a reliable tool for shaping data according to your needs.


# Exception Handling
**Exception Handling in Java**

An exception is like an unexpected guest crashing your code's party, disrupting its flow. It's a runtime hiccup caused by errors, throwing a wrench into your program's smooth operation.

For instance, imagine having flawless-looking code until you run it and encounter an error indicating an attempt to access an index in an array that doesn't exist. This is known as an "array index out of bounds exception."

To address such exceptions, let's create a file on the file system with a path that doesn't exist. Java's File class offers a handy method called "createNewFile," but if the directory doesn't exist, it throws an "IO exception" indicating an issue.

To handle potential errors, enclose the risky code in a try block, indicated by curly braces. Then, introduce a catch block with parentheses and more curly braces. Within these parentheses, specify the type of exception you anticipate, such as "IO exception," and assign it a name, like "E."

Java attempts to create the file, and if it fails and throws an exception, the catch block steps in. You can respond by printing a message, such as "Sorry, an error occurred," ensuring your program doesn't crash.

Beyond printing messages, you can take various actions, like creating the missing directory and retrying the operation. In essence, handling exceptions empowers you to maintain the smooth operation of your program.

# Stack Trace and Exception Message

Exceptions act like messages that reveal what went wrong in our code. One way to gather information from an exception is by using the `getMessage()` method. This method explains why the exception occurred, providing valuable details we can show to users.

For instance, if we encounter an exception named 'e', we can use `e.getMessage()` to retrieve the error message. Running this might display something like "no such file or directory," offering users more insight into the error.

Additionally, exceptions come with a "stack trace," which is like a map showing the path our program followed before encountering the exception. This map aids in pinpointing where things went awry. It's common to print the stack trace when handling an exception, which we achieve using `printStackTrace()`. When executed, it presents a list of classes, methods, and line numbers that led to the exception. You can even click on them for further details.

The last line in the stack trace indicates where the problem originated. For example, it might point to line 11 in a particular method. Each subsequent entry delves deeper into the code, identifying the exact line that caused the issue. Occasionally, you might encounter an entry without a line number, indicating a "native method" written in a language other than Java, which can't be inspected from the stack trace.

At the stack trace's top, you'll find the exception and its message. These messages and stack traces serve as detectives, aiding in identifying the root cause of errors in the code.

# Handling Multiple Exceptions**

When writing code, it's common to encounter various errors, and we need to handle them efficiently. Here are three methods to tackle multiple errors:

1. **Polymorphism:** Think of code errors like a family tree, where "Exception" is the parent and all other errors are its children or grandchildren. Using the parent, "Exception," allows us to catch any error that might occur.

2. **Series of Catch Blocks:** If we know specific types of errors that might arise, such as "FileNotFound" or "InputMismatch," we can put each in separate catch blocks. This allows us to handle different errors differently.

3. **Single Catch Block for Multiple Errors:** Sometimes, different errors might cause the same issue in our code. In such cases, we can streamline our code by using just one catch block to handle them all.

These methods help ensure our code remains robust and resilient to errors, whether they are related like a family, require individual treatment, or cause similar problems.


# 





