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

# 






