# Conditional Statements
> They are also known as decision making statement in java. Sometimes, when we need  to transfer the control of the program to a specified block or location im the program by skipping some lines, we can use conditional statements.

> Eg: if statements, switch cases, loops

### Java if-else Statement
The Java if statement is used to test the condition. It checks boolean
condition: true or false. There are various types of if statement in Java.

- if statement
- if-else statement
- if-else-if ladder
- nested if statement

### If Statement
> It test the particular condition and executes only if that condition is true. 

Syntax
```java
if(condition){
//code executed only if the condition is true
}
```
Example: 
```java
//Java Program to demonstate the use of if statement.  
public class IfExample {  
public static void main(String[] args) {  
    //defining an 'age' variable  
    int age=20;  
    //checking the age  
    if(age>18){  
        System.out.print("Age is greater than 18");  
    }  
  }  
}  
```

### If-Else Statement

> The Java if-else statement also tests the condition. It executes the if block if condition is true otherwise else block is executed.

Syntax
```java
if(condition){  
//code is executed if condition is true  
}
else{  
//code is executed if condition is false  
}  
```
Example: 
```java
public class IfElseExample {  
public static void main(String[] args) {  
    //defining a variable  
    int number=31;  
    //Check if the number is divisible by 2 or not  
    if(number%2==0){  
        System.out.println("even number");  
    }
    else{  
        System.out.println("odd number");  
    }  
  }  
}  
```
### Note: in java we can substitute the if-else block by the ternary operator. 
> We can also use ternary operator (? :) to perform the task of if...else statement. It is a shorthand way to check the condition. If the condition is true, the result of ? is returned. But, if the condition is false, the result of : is returned.

```java
public class IfElseTernaryExample {    
public static void main(String[] args) {    
    int number=31;    
    //Using ternary operator  
    String output=(number%2==0)?"even number":"odd number";    
    System.out.println(output);  
  }    
}    
```

### If-Else-If Statement

> The if-else-if ladder statement executes one condition from multiple statements.


Syntax
```java
if(condition1){  
//code to be executed if condition1 is true  
}
else if(condition2){  
//code to be executed if condition2 is true  
}  
.
.

else{  
//code to be executed if all the conditions are false  
}   
```
Example: 
```java
//It is a program of grading system, D grade, C grade, B grade, A grade and A+. 
public class IfElseIfExample {  
public static void main(String[] args) {  
    int marks=65;  
      
    if(marks<50){  
        System.out.println("fail");  
    }  
    else if(marks>=50 && marks<60){  
        System.out.println("D grade");  
    }  
    else if(marks>=60 && marks<70){  
        System.out.println("C grade");  
    }  
    else if(marks>=70 && marks<80){  
        System.out.println("B grade");  
    }  
    else if(marks>=80 && marks<90){  
        System.out.println("A grade");  
    }
    else if(marks>=90 && marks<100){  
        System.out.println("A+ grade");  
    }
    else{  
        System.out.println("Invalid!");  
    }  
  }  
}    
```


### Nested-If Statement

> The nested if statement represents the if block within another if block. Here, the inner if block condition executes only when outer if block condition is true.


Syntax
```java
if(condition1){    
    //condition1 true, code executed    
    if(condition2){  
       //condition2 true, code executed 
       if(condition3){  
          //condition3 true, code executed    
      }  
    }   
}  
```
Example: 
```java
public class JavaNestedIfExample2 {      
public static void main(String[] args) {      
    //Creating two variables for age and weight    
    int age=25;    
    int weight=48;      
    //applying condition on age and weight    
    if(age>=18){      
        if(weight>50){    
            System.out.println("You are eligible to donate blood");    
        } else{  
            System.out.println("You are not eligible to donate blood");    
        }  
    } 
    else{  
      System.out.println("Age must be greater than 18");  
    }  
  } 
}  

```


## Switch Statements

> They are used for menu driven/User's choice program.

>The Java switch statement executes one statement from multiple conditions. It is like if-else-if
ladder statement. The switch statement works with byte, short, int, long, enum types, String and some wrapper types like Byte, Short, Int, and Long.

In other words, the switch statement tests the equality of a variable against multiple value.

### Important points:
- There can be one or N number of case values for a switch expression.
- The case value must be of switch expression type only. The case value must be literal or constant. It doesn't allow variables.
- The case values must be unique. In case of duplicate value, it renders compile-time error.
- The Java switch expression must be of byte, short, int, long (with its Wrapper type), enums
and string.
- Each case statement can have a break statement which is optional. When control reaches to the break statement
, it jumps the control after the switch expression. If a break statement is not found, it executes the next case.
- The case value can have a default label which is optional.

Syntax
```java
switch(expression){    
case value1:    
 //code to be executed;    
 break;  
case value2:    
 //code to be executed;    
 break;  
......    
    
default:     
  code to be executed if all cases do not matched;  
}   
```
Example: 
```java
// Program to check Vowel or Consonant:
public class SwitchVowelExample {    
public static void main(String[] args) {    
    char ch='O';    
    switch(ch)  
    {  
        case 'a':   
            System.out.println("Vowel");  
            break;  
        case 'e':   
            System.out.println("Vowel");  
            break;  
        case 'i':   
            System.out.println("Vowel");  
            break;  
        case 'o':   
            System.out.println("Vowel");  
            break;  
        case 'u':   
            System.out.println("Vowel");  
            break;  
        case 'A':   
            System.out.println("Vowel");  
            break;  
        case 'E':   
            System.out.println("Vowel");  
            break;  
        case 'I':   
            System.out.println("Vowel");  
            break;  
        case 'O':   
            System.out.println("Vowel");  
            break;  
        case 'U':   
            System.out.println("Vowel");  
            break;  
        default:   
            System.out.println("Consonant");  
    }  
  }    
}     
```

### Why break is important in switch case?
> It executes all statements after the first match if a break statement is not present. This is known as fall through in java.

```java
//Java Switch Example ->  omitting the break statement  
public class SwitchExample2 {  
public static void main(String[] args) {  
    int number=20;  
    //switch expression with int value  
    switch(number){  
    //switch cases without break statements  
    case 10: System.out.println("10");  
    case 20: System.out.println("20");  
    case 30: System.out.println("30");  
    default:System.out.println("Not in 10, 20 or 30");  
    }  
  }  
}  
```

### Nested Switch
We can use switch statement inside other switch statement in Java. It is known as nested switch statement.

```java
public class NestedSwitchExample {    
    public static void main(String args[])  
      {  
      //C - CSE, E - ECE, M - Mechanical  
        char branch = 'C';                 
        int collegeYear = 4;  
        switch( collegeYear )  
        {  
            case 1:  
                System.out.println("English, Maths, Science");  
                break;  
            case 2:  
                switch( branch )   
                {  
                    case 'C':  
                        System.out.println("Operating System, Java, Data Structure");  
                        break;  
                    case 'E':  
                        System.out.println("Micro processors, Logic switching theory");  
                        break;  
                    case 'M':  
                        System.out.println("Drawing, Manufacturing Machines");  
                        break;  
                }  
                break;  
            case 3:  
                switch( branch )   
                {  
                    case 'C':  
                        System.out.println("Computer Organization, MultiMedia");  
                        break;  
                    case 'E':  
                        System.out.println("Fundamentals of Logic Design, Microelectronics");  
                        break;  
                    case 'M':  
                        System.out.println("Internal Combustion Engines, Mechanical Vibration");  
                        break;  
                }  
                break;  
            case 4:  
                switch( branch )   
                {  
                    case 'C':  
                        System.out.println("Data Communication and Networks, MultiMedia");  
                        break;  
                    case 'E':  
                        System.out.println("Embedded System, Image Processing");  
                        break;  
                    case 'M':  
                        System.out.println("Production Technology, Thermal Engineering");  
                        break;  
                }  
                break;  
        }  
    }  
}  

```



















