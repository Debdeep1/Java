## Operators in Java
### Operator in Java is a symbol that is used to perform operations. For example: +, -, *, / etc.

#### There are many types of operators in Java which are given below:
```
- Unary Operator,
- Arithmetic Operator,
- Shift Operator,
- Relational Operator,
- Bitwise Operator,
- Logical Operator,
- Ternary Operator and
- Assignment Operator.
```

### Java Unary Operator
The Java unary operators require only one operand. Unary operators are used to perform various operations i.e.:

- incrementing/decrementing a value by one
- negating an expression
- inverting the value of a boolean

Java Unary Operator Example: ++ and --
```java
public class OperatorExample{  
public static void main(String args[]){  
int x=10;  
System.out.println(x++);//10 (11)  
System.out.println(++x);//12  
System.out.println(x--);//12 (11)  
System.out.println(--x);//10  
}}  
```

### Java Arithmetic Operators
Java arithmetic operators are used to perform addition, subtraction, multiplication, and division. They act as basic mathematical operations.

#### Java Left Shift Operator
The Java left shift operator << is used to shift all of the bits in a value to the left side of a specified number of times.

#### Java Right Shift Operator
The Java right shift operator >> is used to move the value of the left operand to right by the number of bits specified by the right operand.

#### Java AND Operator Example: Logical && and Bitwise &
The logical && operator doesn't check the second condition if the first condition is false. It checks the second condition only if the first one is true.

The bitwise & operator always checks both conditions whether first condition is true or false.

#### Java OR Operator Example: Logical || and Bitwise |
The logical || operator doesn't check the second condition if the first condition is true. It checks the second condition only if the first one is false.

### Java Ternary Operator
##### Java Ternary operator is used as one line replacement for if-then-else statement and used a lot in Java programming. It is the only conditional operator which takes three operands.

Java Ternary Operator Example
```java
public class OperatorExample{  
public static void main(String args[]){  
int a=2;  
int b=5;  
int min=(a<b)?a:b;  
System.out.println(min);  
}}  
```

### Java Assignment Operator
##### Java assignment operator is one of the most common operators. It is used to assign the value on its right to the operand on its left.
