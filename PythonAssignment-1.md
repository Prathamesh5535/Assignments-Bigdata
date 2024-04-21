Q1. Why do we call Python a general-purpose and high-level programming language?
Python is considered a general-purpose language because it can be used for a wide range of applications, from web development and data science to artificial intelligence and automation. It's high-level because it abstracts many complex details away from the programmer, making it easier to write and understand code.

Q2. Why is Python called a dynamically typed language?
Python is called a dynamically typed language because variable types are determined at runtime, rather than being explicitly declared in code. This means you can assign different types of values to the same variable without any explicit type declaration.

Q3. List some pros and cons of Python programming language?
Pros:

Readable and clean syntax
Large standard library
Strong community support
Cross-platform compatibility
Extensive third-party libraries for various tasks
Cons:

Slower execution speed compared to compiled languages
Global interpreter lock (GIL) can limit concurrency
Not as suitable for high-performance computing or low-level system tasks
Q4. In what all domains can we use Python?
Python can be used in various domains including:

Web development
Data science and machine learning
Artificial intelligence and robotics
Desktop GUI applications
Game development
Network programming
Scripting and automation
Q5. What are variables and how can we declare them?
Variables are containers for storing data values. In Python, you can declare a variable by simply assigning a value to a name. For example:

python
Copy code
x = 5
name = "John"
Q6. How can we take input from the user in Python?
You can take input from the user using the input() function. For example:

python
Copy code
user_input = input("Enter something: ")
Q7. What is the default datatype of the value that has been taken as an input using input() function?
The input() function always returns a string, regardless of what the user enters.

Q8. What is type casting?
Type casting is the process of converting the datatype of a value from one type to another. Python provides built-in functions like int(), float(), str(), etc., for type casting.

Q9. Can we take more than one input from the user using a single input() function? If yes, how? If no, why?
No, you can't take multiple inputs directly using a single input() function. However, you can take a single input and then split it based on some delimiter to get multiple values.

Q10. What are keywords?
Keywords are reserved words in Python that have special meanings and purposes. They cannot be used as identifiers (variable names, function names, etc.).

Q11. Can we use keywords as a variable? Support your answer with a reason.
No, you cannot use keywords as variable names because they are reserved for specific purposes in Python. Attempting to use a keyword as a variable name will result in a syntax error.

Q12. What is indentation? What's the use of indentation in Python?
Indentation refers to the spaces or tabs at the beginning of a line of code to define a block of code. In Python, indentation is used to denote the beginning and end of control flow structures like loops, conditional statements, and function definitions. It's not just for readability; Python actually uses indentation to determine the structure of the code, unlike other languages where curly braces or keywords are used.

Q13. How can we throw some output in Python?
You can output data in Python using the print() function. For example:

python
Copy code
print("Hello, world!")
Q14. What are operators in Python?
Operators in Python are special symbols or keywords that perform operations on operands. They include arithmetic operators (+, -, *, /, etc.), comparison operators (==, !=, <, >, etc.), logical operators (and, or, not), assignment operators (=, +=, -=, etc.), and more.

Q15. What is the difference between / and // operators?
The / operator performs regular division, returning a floating-point result, while the // operator performs floor division, returning the quotient as an integer (rounded down to the nearest whole number).

Q16. Write a code that gives the following as an output.

Copy code
iNeuroniNeuroniNeuroniNeuron
Here's the code:

python
Copy code
print("i" + "Neuron" * 4)
Q17. Write a code to take a number as an input from the user and check if the number is odd or even.

python
Copy code
num = int(input("Enter a number: "))
if num % 2 == 0:
    print("Even")
else:
    print("Odd")
Q18. What are boolean operators?
Boolean operators in Python are used to perform logical operations on boolean values. They include and, or, and not.

Q19. What will be the output of the following?

graphql
Copy code
1 or 0
0 and 0
True and False and True
1 or 0 or 0
The outputs will be:

graphql
Copy code
1
0
False
1
Q20. What are conditional statements in Python?
Conditional statements in Python allow you to execute different blocks of code based on certain conditions. They include if, elif (short for "else if"), and else.

Q21. What is the use of 'if', 'elif', and 'else' keywords?

if: It is used to check a condition and execute a block of code if the condition is true.
elif: It is used to check additional conditions if the preceding if or elif conditions are false.
else: It is used to execute a block of code if none of the preceding conditions are true.
Q22. Write a code to take the age of a person as an input and if age >= 18 display "I can vote". If age is < 18 display "I can't vote".

python
Copy code
age = int(input("Enter your age: "))
if age >= 18:
    print("I can vote")
else:
    print("I can't vote")

 Q23. Write a code that displays the sum of all the even numbers from the given list.

python
Copy code
numbers = [12, 75, 150, 180, 145, 525, 50]
sum_even = 0
for num in numbers:
    if num % 2 == 0:
        sum_even += num
print("Sum of even numbers:", sum_even)
Q24. Write a code to take 3 numbers as an input from the user and display the greatest number as output.

python
Copy code
num1 = float(input("Enter first number: "))
num2 = float(input("Enter second number: "))
num3 = float(input("Enter third number: "))
print("The greatest number is:", max(num1, num2, num3))
Q25. Write a program to display only those numbers from a list that satisfy the following conditions:

The number must be divisible by five
If the number is greater than 150, then skip it and move to the next number
If the number is greater than 500, then stop the loop
python
Copy code
numbers = [12, 75, 150, 180, 145, 525, 50]
for num in numbers:
    if num > 500:
        break
    if num > 150:
        continue
    if num % 5 == 0:
        print(num)   