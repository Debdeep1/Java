# Introduction to Programming Languages
## What are programming langauges?
Programming languages, internally are basically binary instructions(if you go into minutest details).
They are used to instruct(instructions read and processed by the CPU) a computer to perform a particular task.


## Why programming languages? Why not simply use the binary instructions?
It is a very difficult task to manually send binary instructions. So to have a human readable format, as well as computer readable architecture, we use programming languages that convert your code(source code) to machine code(binary instructions).


### Types of programming languages:

1. Procedural Language
They specify a series of well-structured steps and procedures to compose a program.
They contain a systematic order of statements, functions, and commands to complete tasks.
What I mean by this is, computer will not say:
"Input 1st number" ==> "Find sum of 2 numbers" ==> "Input 2nd number"
This is not procedural/sequential.

`Example:` C language, all other languages. Since every language follows the procedural format(sudden change/irrational instructions are not executed)


2. Functional Language
Writing a program only in pure functions or simple modules, i.e. never modify variables(a=10 doesnt become a=Jack), only create new outputs </br>
Mainly used in situations where we have to consider and perform on lots of different operations on the same set of data. </br>
Write a block of functions and use/reuse it multiple times to perform different set data. </br>
Meaning: </br>
to find sum of 10 pair of numbers. </br>
Find sum of 1st pair.
==> If the code is correct, then reuse the function(block/set of code)to perform same operation on the rest data. </br>
==> If the code is incorrect, then you dont have to change it for 10 pairs... just change for 1 pair rest automatically is fixed. </br>
Follow the rule of First Class Functions: reassigning value of a variable to another variable
(e.g. in python, a=10, b=20, c=b  ==> you are assigning the value of a variable to another variable. This is the property of a first class function. Example of First Class Function language-> Python)


3. Object Oriented Programming Language
What is a object?
Suppose we create a collection of data with roll numbers of all the students...what is the type of the data? Integers(numbers)
Similarly if we collect the data of all students(with 3 properties: name, roll number, grades)
Now this is both a String(text/paragraph type) as well as Integer(number) or Character(grades A B C...)
This can be taken under custom data type! We can specify these custom data types using classes...
Classes: Named group of properties and functions...(we'll learn more about classes in the future)
Class is like a property/template...I am an object of human class; roll number is an object(instance) of the class student!
If we save int a = 10;  A is the variable, int is the data type/ class and 10 is the object of integer type...


Mainly revolves around objects
Function(code) + Data = Object
Divide a code into various chunks, so that it is easier for us to develop,debug,reuse and maintain the software.


Let's say we want to change the type of data in a program; suppose we want to change the steering wheel...we dont change the entire car...we change the object of the car...(in simple terms)

`Example:` Java and Python

If a particular programming language follows one stereotype, doesnt mean it won't follow the others...
Java can be both procedural and oop... python can do all.

Compile meaning: to translate instructions from one computer language into another for a computer to understand
(source code to machine code)

### Static vs Dynamic Languages

Static			|			Dynamic
------------|------------
Perform type checking at compile time		|  Perform type checking at runtime
Errors will show at compile time		    |  Error might not show till program runs
Declare datatype before you use it	|	No need to declare datatype of variables
More controlled			|		Saves time in writing code but might give errors at runtime
int a=10(passed)		|		a=kunal(passed)
int a=John(error)		|		int a=10(passed)


### Errors in Static Languages

a=10
a="John"

This will not give an error in dynamic languages, because the value at compile time changes from 10 to John...
This does not occur due to concepts of objects and references via which the value of the object was updated at runtime to the new value.

But in static languages it will show an error, as we declared the data type to be int but then we assign a string(text)value to this object. This will throw a compile time error(type mismatch error)

'a' + 10
Will throw an error in static languages

# Memory Management
