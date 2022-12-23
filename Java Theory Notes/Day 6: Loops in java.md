## LOOPS in JAVA
### What are loops?
> Loops are statements used to run a particular block of code for n number of times till the desired result is obtained.
 
 E.g
- Print a number 1000 times.
- We cannot manually print them out 1000times...
- So we use looping statements to perform these tasks automatically, till a certain condition is met.
___
### How many types of loops?
 1. For loop.
 2. While loop.
 3. Do while loop.
 
### Syntax for 1. For loop:
```java
 for(initialisation; condition; increment/decrement control)
 {
 	//code block or body to execute
 }
```
> ### Q 1.) Print numbers from 1 to 5
```java
  for(int i=1;i<=5;i++)
  	{
  		System.out.print(i+"\t");
  	}
```
> - Whenever the loop executes, i gets initialised to 1. <br/>
> - After that it checks if i satisfies the given condition, i.e. i is less than or equal to 5. <br/>
> - For true case, the control variable is incremented by 1.
> - <br/> For false case, the loop is not executed any more.
> - <br/> For each of the true cases, the body of the loop executes and a number is printed out.
> - <br/> After execution, the value increments and the checking continues.
 ##### Algorithm:
- 1st time-> initialise->check->increment/decrement <br/>
- 2nd time onwards-> no more initialisation, update and store value-> check-> increment/decrement <br/>
- Last time->checking fails->control moves out of the loop-> no more loop executed. <br/>
  
> ### Q 2.) Print numbers from 0 to 30
> ### Q 3.) Accept the a number from user and print numbers from 1 to that number.
___
### Syntax for While loop:
```java
  while(condition){
	//body
	increment/decrement control variable
}
```
#### Q 1.) ans in while loop
```java
int num = 1;
while(num<=5)
{
	System.out.println(num+"\t");
	num++;
}
```

> ### Q 4.) Print odd numbers less than 10
___
#### When to use while and when to use for loop?
> Run while loop when you dont know how many times a loop will run(also known as entry controlled loop) <br/>
- e.g. keep taking input from the user till the user presses 'x' <br/>
> Run the for loop when you know how many times a loop is going to run <br/>
- e.g. keep printing numbers in a certain range <br/>
___
### Syntax for Do while loop:
#### This is an exit controlled loop. So it will execute atleast once, and then check if the condition is true. In such cases, while loops may not execute but do while will execute for once. 
```java
do{
	do this...block execution
}
while(condition);
```
#### Q 1.) ans in do while loop
```java
int n = 1;
 do{
 	System.out.println(n);
 	n++;
 }
 while(n<=5);
```
 Example of execution atleast once
```java
int n = 1;
do {
	System.out.println("Hello world");
}
while(n!=1);
```
> #### This will still run and print once, even if n is equal to 1.
