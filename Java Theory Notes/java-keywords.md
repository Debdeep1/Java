## Example 1
public class program1 </br>
{		      </br>
	public static void main(String[]args)  </br>
	{					</br>
		System.out.println("Hello World");	</br>
	}					</br>
}			</br>


## keywords, indentifiers, literals, punctuators and operators make up for a java statement.

### Access specifiers, return types and modifiers

 - Access specifiers-> public, private, protected and default
 - 1st public meaning->
this class can be accessed from anywhere, in the entire program.

#### if the name of the file is pro.java then the class name has to be class pro!

 - main function-> the word is reserved. If the function name isn't set to main, your execution will stop. Whenever you execute a program, java will look for the main function in the code.
##### [Entry point of the java program]

 - 2nd public-> if the function has an important role in the code, it should be accessible publicly for the execution.
Main will not be able to run if the function is made private.

 - static-> in order to use the variables of a class, globally, you need to make objects of the class
if the object itself is not available to the user, then the desired task cannot be performed.
There can be 2 types of instances/objects-> static and non-static
e.g.-> static int a;(static)   &&   int a;(non-static)

 - void-> return type of the value.

 - String[]args-> command line arguements-> These are array type arguements in the form of collection of strings.
Sopln(args[0]);

 - Sopln-> Java developers created some predefined and precompiled functions and classes to perform specific tasks.
E.g.-> System class -> imported into the java program by default as a part of java.lang package
out-> is a print stream which will print the output as a stream of data values.

## Example 2

import java.util.Scanner;	</br>
import java.io.*;	</br>
class Main	</br>
{	</br>
    public static void main(String[]args) </br>
    { </br>
        Scanner sc = new Scanner(System.in); </br>
        System.out.println("Enter a name"); </br>
        String name = sc.next(); // sc.nextLine();          </br>
        System.out.println("Enter a value"); </br>
        int a = sc.nextInt(); </br>
        System.out.println(name+" "+a); </br>
    } </br>
} </br>
