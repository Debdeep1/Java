## Example 1

```java
public class Program{
    public static void main(String[] args){
	System.out.println("Hello World");
    }
}

```
 - keywords, indentifiers, literals, punctuators and operators make up for a java statement.

### What is public?
> public: is an access-modifier or access-specifier or a visibility-specifier which can be accessed anywhere in the entire program whether inside or outside the class or package.

- Types of Access specifiers ->
 ```public, private, protected and default```
	- public: mentioned above
	- private:  Private access modifier allows the least accessibility with the private data members to be accessible only within the class.
	- protected: Protected visibility specifier allows access only to subclasses inheriting the class in which protected members are declared. 
	- When no access modifier is specified for a class, method, or data member – It is said to be having the default access modifier by default. 
	
![Screenshot from 2022-12-02 17-36-02](https://user-images.githubusercontent.com/66300439/205289291-5d9ca965-787e-4c84-957b-9bd4c8d321cb.png)

## What is class?
> class is a group of objects and functions.

### Note: if the name of the file is pro.java then the class name has to be class pro!

## What is a main()?
 > Main function-> the word is reserved. If the function name isn't set to main, your execution will stop. Whenever you execute a program, java will look for the main function in the code. Entry point of the java program


## What is a static?
 > static-> in order to use the variables of a class, globally, you need to make objects of the class, if the object itself is not available to the user, then the desired task cannot be performed.
There can be 2 types of instances/objects-> static and non-static

e.g:  static int a;(static)   &&   int a;(non-static)
```java
class Student
{
int roll_no;
float marks;
String name;
static String College_Name="ITM";
}
class StaticDemo
{
public static void main(String args[])
{
Student s1=new Student();
s1.roll_no=100;
s1.marks=65.8f;
s1.name="abcd";
System.out.println(s1.roll_no);
System.out.println(s1.marks);
System.out.println(s1.name);
System.out.println(Student.College_Name); 
//or System.out.println(s1. College_Name); but first is use in real time.
Student  s2=new  Student();
s2.roll_no=200;
s2.marks=75.8f;
s2.name="zyx";
System.out.println(s2.roll_no);
System.out.println(s2.marks);
System.out.println(s2.name);
System.out.println(Student.College_Name); 
}
}
```

## What is void? 
> void:  return type of the funtion. void doesn't return any value. 

## Whats is String[] args?
> String[]args: These are basically command line arguements which means whatever arguement to give in the terminal while running it will store it in a form of string array. These are array type arguements in the form of collection of strings.
Sopln(args[0]);

## Whats is System.out.println?
 - System.out.println / System.out.print-> Java developers created some predefined and precompiled functions and classes to perform specific tasks.

E.g.-> System class -> imported into the java program by default as a part of java.lang package

out-> is a print stream which will print the output as a stream of data values.

## Datatypes in Java
- Primitive: 
	- boolean: stores true or false
	- char: stores character like a , b, $, @ etc. The char data type is a single 16-bit Unicode character. It has a minimum value of '\u0000' (or 0) and a maximum value of '\uffff' (or 65,535 inclusive).
	- byte: It is a 8 bit signed 2's complement integer. It has a minimum value of -128 and a maximum value of 127 (inclusive).
	- short: Stores whole numbers from -32,768 to 32,767
	- int: Stores whole numbers from -2,147,483,648 to 2,147,483,647
	- long: Stores whole numbers from -9,223,372,036,854,775,808 to 9,223,372,036,854,775,807
	- float: It is a 32bit IEEE 754 floating point stores decimal numbers  from 1.175494351 E - 38 to 3.402823466 E + 38.
	- double: It is a 64bit IEEE 754 floating point stores decimal numbers from 2.2250738585072014 E - 308	to 1.7976931348623158 E + 308
- Non-Primitive: 
	- Classes
	- Interfaces
	- Arrays 
### Note: 8-bit = 1 byte
![Screenshot from 2022-12-02 18-03-55](https://user-images.githubusercontent.com/66300439/205293963-2827ce7d-a88a-48e5-9d10-d41017fad129.png)


## How to take inputs? 
```java
import java.util.Scanner;	
import java.io.*;	
class Main	
{	
    public static void main(String[]args)
    { 
        Scanner sc = new Scanner(System.in);
        System.out.println("Enter a name"); 
        String name = sc.next(); // sc.nextLine();       
        System.out.println("Enter a value"); 
        int a = sc.nextInt();
        System.out.println(name+" "+a); 
    } 
} 
```
____
# Questions
### Write a program in java to input 3 numbers and calulate the sum and average of it.
```java
import java.util.Scanner;
import  java.io.*;

public class program {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.println("Enter 1st number");
        int num1 = sc.nextInt();
        System.out.println("Enter 2nd number");
        int num2 = sc.nextInt();
        System.out.println("Enter 3rd number");
        int num3 = sc.nextInt();

        System.out.println("Sum = " + (num1+num2+num3));
        double avg = (num1+num2+num3)/3;
        System.out.println("Average = " + avg);
    }
}

```

### WAP in java to take name as input and print a greeting message for that particular name.
```java
import java.util.Scanner;
/*
Input: Soumali
Output: Good morning, Soumali!
 */

public class Geetings {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.println("Enter a name");
        String name = sc.nextLine();
        System.out.println("Good morning, " + name + "!");
    }
}
```

### Write a program in java to input principal, time, and rate (P, T, R) from the user and find Simple Interest.


