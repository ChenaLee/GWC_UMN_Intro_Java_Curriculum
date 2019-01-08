# 00_What_is_programming
## Counting from Zero - Zero Based Numbering
Did you notice this is marked as lesson **00** intead of **01**?  
In programming, most of times countring and numbering starts from *Zero*.  
It's a convention among mathematicians and computer scientists.   

### Exercise 1
> Lined up with a group of classmates.  
>  
>  Line: | A | B | C | D | You | E | F  
> -- | -- | -- | -- | -- | -- | -- | --
> Non-programmers | 1 | 2 | 3 | 4 | 5 | 6 | 7
> Programmers | 0 | 1 | 2 | 3 | 4 | 5 | 6  
>  
> You are at position 4, not 5!  

## So what is Programming? 
### Analogy 1
* Let's assume in **Human** only speaks **English**. But can easily learn **Spanish** if they try. Learning **Chinese** is much more difficult.  
* **google translator** only knows show to convert **Spanish** into **Chinese**.  
* **Computer** only speaks **Chinese**.  
* **Programmers** are people who learned how to speak Spanish. Even though they think in English, they can write in Spanish.  

Then they would do the following to communicate.  
**English** > Write > Instruction in **Spanish** > Google Translate > Instruction in **Chinese**
 
Equivalent of this in technological terms is:  
**Natural Language** > Coding/Programming > **Code in High Level Programming Language** > Compiler Compiles > **Machine Code**

When we say "running a program", it's like giving the instruction in Chinese you have to the computer so the computer can do what it is told to do.

There are many programming languages you can use to make **Code in High Level Programming Languages**. One of the most popular ones is **Java**, which you will learn and use throughout the class.  

## Print and Run your first program
### Get your environment ready
1. Open Eclipse IDE
2. File -> New -> Java Project -> "GwcS2019{YourName}" as project name
3. If src folder doesn't exist, File -> New -> Source Folder -> Create a "src" folder using your project name.
4. File -> New -> Class -> "HelloWorld" as class name. Check the box saying "public static void main(String[] args)". Don't worry about what those words mean yet!

### What is Print?
If you make a text messaging app, users will open(run) the app, and your code will display some messages sent to that user.  
To make that happen, you will need a screen to show your messages first, right?  
In programming, **Console** is the default screen you can show your one-way messages on.  
Console can also take inputs from you, but let's focus on "showing messages" part for now.  

### Printing "Hello world!"
"Hello world" is how pretty much every programmer starts their programming journey. After this exercise, you are a part of the programmer community!  
1. In the class file you just created, in main, put **System.out.println("Hello world!");**
System.out.println() print whatever you give in the brackets to the Console, so users can see it - because users can't read your code!  
2. Double check you have the semicolon at the end! In Java, it's like a "period" mark at the end of an english sentence. It might look weird right now, but you will get used to it!
3. File -> Save (or press ctrl+s)
4. Right click on your class in the Package Explorer (on the LHS) -> Run As -> Java Application.
5. Verify that the "console" in the bottom of Eclipse says "Hello world!"
For example, your class would look like:
```
package GwcS2019Chena;

public class HelloWorld {

	public static void main(String[] args) {
		System.out.println("Hello world!");
	}

}
```
