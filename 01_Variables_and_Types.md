# 01_Variables_and_Types
## Variables
### Variables - Analogy
Variable is something that can change. The name is fairly self-explanatory, right?  
@TODO

+------+    +------+
|  x   |    |  y   |
+------+    +------+


### Variables in Mathematics
@TODO

### Varaibles in Programming
@TODO
name of variable and value

## Types
### Types - Analogy
@TODO
boxes of different shapes!

### Common Types in Programming - Primitive Types
List of types

#### int
@TODO

#### double
@TODO

## Equal Sign - Assignment and Comparison
### Equal Sign in Mathematics
@TODO

### Equal Sign in Programming
kind of like arrow

### Comparison in Programming
Then how do we say two things are equal in programming?  
== sign  

## Mathematical Operators
Addition uses "+". e.g. 1+2  
Subtracion uses "-". e.g. 2-1  
Multiplication uses "*". e.g. 2*3  
Division uses "/". e.g. 1/2  

## Learn And Exercises
### Recap: Create a class named "Variables" in the project you created from lesson 0 in the same way.
Review lesson 0 if this is difficult.

### Exercise 0 : Two variables with different types.
When you first *create* a variable, you specify its type. It is a good idea to also *initialize* the variable with a value.  
This is called *declaration*, or *to declare a variable*. Here is an example of how you *declare an int* and *assign* it a value.
```
int myInt = 0;
```
*myInt* is a name of the variable, *int* is its type, and 0 is its current value.  


1. In main function, create an int type variable named *number* with value 1. Print it. Try running it!  
2. Follwing 1, create a double type variable named *doubleNumber* with value 1.3. Print it. Try running it!  

e.g.
```
package GwcS2019Chena;

public class Variables {

	public static void main(String[] args) {
		int number = 1;
		System.out.println(number);
		
		double doubleNumber = 1.3;
		System.out.println(doubleNumber);
	}
}
```

Results in console:
```
1
1.3
```

### Exercise 1 : Changing values in a variable.
You can change a value of a variable you declared already. That's why it's called a *variable*!

Continue in the same funciton you coded in exercise 0.
1. Change the value of *number* to 2. Print it. Try running it!
2. Change the value of *doubleNumber* to 2.5. Print it. Try running it!

e.g.
```
public class Variables {

	public static void main(String[] args) {
		int number = 1;
		System.out.println(number);
		
		double doubleNumber = 1.5;
		System.out.println(doubleNumber);
		
		number = 2;
	    	System.out.println(number);
	    
	    	doubleNumber = 2.5;
	    	System.out.println(doubleNumber);
	}
}
```

Results in console:
```
1
1.3
2
2.5
```

### Exercise 2 : Two variables with incompatible values. Commenting Code
1. Create another int type variable named "anotherNumber* with value 2.3. What happened?
> You should be seeing a red line on your code. Hover your mouse over it. Can you explain why that happened?
> int type variable cannot take non-integer value! If you try running your code, what happens?
2. Putting // in front of each line let you *comment* your code. This means the line is a comment for human, and computer won't run that line. Try putting // in front of the line that just errored out. Can you run your code now?
3. Create another double type variable named "anotherDoubleNumber* with value 2. Print it. Try running it! What happened?  
> Can you see it printed 2.0 instead of 2? Can you explain why that happened?

e.g.
```
//int anotherNumber = 2.3;
double anotherDoubleNumber = 2;
System.out.println(anotherDoubleNumber);
```

Results in console:
```
2.0
```

### Exercise 3 : Mathematical Operators
Print can take an operation as well. For example, you can do
```
System.out.println(x+2);
```

1. Print number+1, doubleNumber-1, number*2, and doubleNumber/2
2. Print number and doubleNumber again. Did they change? Why not?

e.g.
```
System.out.println(number+1);
System.out.println(doubleNumber-1);
System.out.println(number*2);
System.out.println(doubleNumber/2);

System.out.println(number);
System.out.println(doubleNumber);
```

Results in console:
```
3
1.5
4
1.25
2
2.5
```

### Exercise 4 : Modifying value of a variable using operation
You can modify a vairable using operation. For example, **x=x+1** will take x value, add 1 to it, and save it back into x. If x was 2 in the beginning, after **x=x+1**, x will become 3.
1. Try the following code snippet and explain what happened, and why it happened. You will see a type mismatch.
```
number = doubleNumber+2;
```
2. Now instead, increase doubleNumber's value by 2 and save it back into doubleNumber. Print it. Did it change from what it was before?
e.g.
```
doubleNumber = doubleNumber+2;
System.out.println(doubleNumber);
```
Results in console:
```
4.5
```
