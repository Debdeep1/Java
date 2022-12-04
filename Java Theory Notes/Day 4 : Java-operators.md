## Operators in Java
### Operator in Java is a symbol that is used to perform operations. For example: +, -, *, / etc.

#### There are many types of operators in Java which are given below:
```
- Unary Operator,
- Arithmetic Operator,
- Assignment Operator.
- Relational Operator,
- Logical Operator,
- Bitwise Operator,
- Ternary Operator

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
> Java arithmetic operators are used to perform addition, subtraction, multiplication, and division. They act as basic mathematical operations.
> eg: +,-.*,/,%
```java
class Main {
  public static void main(String[] args) {
    
    // declare variables
    int a = 12, b = 5;

    // addition operator
    System.out.println("a + b = " + (a + b));

    // subtraction operator
    System.out.println("a - b = " + (a - b));

    // multiplication operator
    System.out.println("a * b = " + (a * b));

    // division operator
    System.out.println("a / b = " + (a / b));

    // modulo operator
    System.out.println("a % b = " + (a % b));
  }
}
```

### Java Assignment Operator
> Java assignment operator is one of the most common operators. It is used to assign the value on its right to the operand on its left.

| Operator | Example | Equivalent |
| :---         |     :---:      |          ---: |
| =  | a = b |	a = b |
| += |  a += b | a = a + b |
| -= |	a -= b | a = a - b |
| *= |	a *= b |	a = a * b |
| /= |	a /= b |	a = a / b |
| %= |	a %= b |	a = a % b |

```java
class Main {
  public static void main(String[] args) {
    
    // create variables
    int a = 4;
    int var;

    // assign value using =
    var = a;
    System.out.println("var using =: " + var);

    // assign value using =+
    var += a;
    System.out.println("var using +=: " + var);

    // assign value using =*
    var *= a;
    System.out.println("var using *=: " + var);
  }
}
```


### Java Relational Operators: !=, ==, >,<,>=,<= :-
> These operators are used to derive relation between arguments in a statement.

| Operator | Description | Example |
| :---         |     :---:      |          ---: |
| ==   | Is Equal To | 3 == 5 returns false |
| !=    | Not Equal To | 3 != 5 returns true |
| >    | Greater Than | 3 > 5 returns false |
| <   | Less Than | 3 < 5 returns true |
| >=    | Greater Than Equal to | 3 >= 5 returns false |
| <=    | Less Than Rqual To | 3 <= 5 returns true |


```java
class Main {
  public static void main(String[] args) {
    
    // create variables
    int a = 7, b = 11;

    // value of a and b
    System.out.println("a is " + a + " and b is " + b);

    // == operator
    System.out.println(a == b);  // false

    // != operator
    System.out.println(a != b);  // true

    // > operator
    System.out.println(a > b);  // false

    // < operator
    System.out.println(a < b);  // true

    // >= operator
    System.out.println(a >= b);  // false

    // <= operator
    System.out.println(a <= b);  // true
  }
}
```
- Note: Relational operators are used in decision making and loops.


### Java Logical Operators: &&, ||, ! :- 
> These operators are used to check for a logical relation in a statement. 

| Logical &&  | Bitwise & |
| ------------- | ------------- |
| The logical && operator doesn't check the second condition if the first condition is false. It checks the second condition only if the first one is true.  | The bitwise & operator always checks both conditions whether first condition is true or false. |

```java
class Main {
  public static void main(String[] args) {

    // && operator
    System.out.println((5 > 3) && (8 > 5));  // true
    System.out.println((5 > 3) && (8 < 5));  // false

    // || operator
    System.out.println((5 < 3) || (8 > 5));  // true
    System.out.println((5 > 3) || (8 < 5));  // true
    System.out.println((5 < 3) || (8 < 5));  // false

    // ! operator
    System.out.println(!(5 == 3));  // true
    System.out.println(!(5 > 3));  // false
  }
}
```
#### Java Left Shift Operator
> The Java left shift operator << is used to shift all of the bits in a value to the left side of a specified number of times.

#### Java Right Shift Operator
> The Java right shift operator >> is used to move the value of the left operand to right by the number of bits specified by the right operand.


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
## Questions
### Q) int a = 2, b = 3, c = 0; Find c where c = ++a - --b;
```
c = 3 - (2) //++a = ++2 -> 3, --b = --3 -> 2 
c = 1
```
### Q) int a = -4, b = 7, c = 0; Find c where c += ++a - b++ -a;
```
c = c + ++a - b++ -a
c = 0 + -3 -7 -(-3) //++a = -3, b-- = first write the value of b and then do b++ -> 8, a = -3
c = 0 + -3 -7 +3
c = -7
```
 # Homework (do not use any conditionals or loop statements)
 ___

### Q) Length and breadth of a rectangle are 5 and 7 respectively. Write a program to calculate the area and perimeter of the rectangle.
 ___
### Q) Suppose the values of variables 'a' and 'b' are 6 and 8 respecrtively, write two programs to swap the values of the two variables. 
###  1 - first program by using a third variable
###  2 - second program without using any third variable
### ( Swapping means interchanging the values of the two variables E.g.- If entered value of x is 5 and y is 10 then after swapping the value of x and y should become 10 and 5 respectively.)
 ___
### Q) Write a program to reverse a 3-digit number. E.g.-Number : 132        Output : 231
