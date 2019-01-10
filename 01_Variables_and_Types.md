# 01_Variables_and_Types
## Variables
### Variables - Analogy
Variable is something that can change. The name is fairly self-explanatory, right?  
@TODO

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
int myInt = 0.
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
		
		double anotherNumber = 1.3;
		System.out.println(anotherNumber);
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
2. Change the value of *anotherNumber* to 2.5. Print it. Try running it!

e.g.
```
package GwcS2019Chena;

public class Variables {

	public static void main(String[] args) {
		int number = 1;
		System.out.println(number);
		
		double anotherNumber = 1.3;
		System.out.println(anotherNumber);
    
    number = 2;
    System.out.println(number);
    
    anotherNumber = 2.5;
    System.out.println(anotherNumber);
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

### Exercise 2 : Two variables with imcompatible values.
1. Create another int type variable named "anotherNumber* with value 2.3. Print it. Try running it! What happened?  
2. Create another double type variable named "anotherDoubleNumber* with value 2. Print it. Try running it! What happened?  

### Exercise 3 : Addition and Subtraction
1. 
2.
3. Re-assignment of variable x = x+1  

### Exercise 4 : Multiplication and Division



exercise4: save it number+anotherNumber to a double, number+doubleNumber to int,
Challege: By re-using only one variable called "myNumber" and a string, print your age, , then your age
Challenge2: something about char and string..


