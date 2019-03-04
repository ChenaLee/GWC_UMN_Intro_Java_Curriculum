# 04 Looping Structures

## Looping in Java

A loop in programming language is a way of writing code in such a way that allow us to run a block of code in a finite and determined amount of time. 

An example of this would be that you would be that we want to draw a right-angle triangle made out of "#" on our console. 

```
#
# #
# # #
# # # #
# # # # #
# # # # # #
# # # # # # #
```

One way to do this is to write seven lines of:

```
System.out.println("#");
System.out.println("# #");
System.out.println("# # #");
System.out.println("# # # #");
System.out.println("# # # # #");
System.out.println("# # # # # #");
System.out.println("# # # # # # #");
```

This is very inefficient and tedious and we would like to write some code that is both smarter, easier to read, and more efficient.

Here's an example of something we can write and by the end of the class you can write one yourself as well. (If you don't know what String is and how they work, go here ....)

```
for (int row = 0; row <= 7; row++){
	String line = '';
	for (int col = 0; col < row; col++) {
		line = line + " #";
	}
	System.out.println(line);
}
```

## Structures / Components

Loop structure is the name we give to different variantion of loops that we can write and each of them will work in a sightly different manner but the same concept still apply, we are trying to run a block of code multiple times.

Now we will explain each of the components that comes into making a loop:

* Counter - A variable that we use to help us manage our loop.  
* Initialization - Use to create our counter and giving it a value.  
* Loop-condition - Use to determine whether we should continue with the loop or terminate it base on our counter.    
* Modifiers - What we do to our counter every loop.  
* Statment(s) - What we want to run every loop.  

Every loop structures in Java must contains all of these components. Now that we are moving on to discussing each of the structure you will see a diagram indicating how our code will flow through each of the compoenents for each structure.

### For Loop

![alt text](https://github.com/ChenaLee/GWC_UMN_Intro_Java_Curriculum/blob/master/images/For_Loop_Diagram.png "For Loop Diagram")

For loop is the most basic of all the structure and the easiest one to follow. We will go through this block of code and see how it actually works.

```
for (int counter = 0; counter <= 3; counter ++){
	System.out.println(counter);
}
```
First let's identify each of our components:

* Counter = `counter` This is the variable we will be using to mange our loop.
* Initialization = `int counter = 0` We assign our variable `counter` with the number 0.  
* Loop-condition = `counter <= 3` This mean that our loop will stop when counter is not less than or equal to 3.  
* Modifiers = `counter++` This mean that for each of our loop we will increase counter by 1.  
* Statement = `System.out.println(counter)` This is what we want to do every loop, we will print out our variable `counter`

So how does the loop work ? Let's go through it (Use the diagram for help):

1. We first initalize our counter.
2. Then we look to see if our condition fail or not. If it doesn't we continue to our statments.
3. We run our statements.
4. We then modify our variable using the modifier.
5. Now we check if our condition fail or not again. 
	* If it fail then we skip our statements and our for loop end
	* if it doesn't fail we go to our statements and continue with our loop.

#### Exercise 0: Practice with For Loop

Let's start of with something simple.  
What would the output of the for loop we discussed about previously be ?

```
for (int counter = 0; counter <= 3; counter ++){
	System.out.println(counter);
}
```
Once you are done with your guess, let's run the code and see if you are correct.

```
package GwcS2019Chena;

public class Loops {
	public static void main(String[] args) {
		for (int counter = 0; counter <= 3; counter ++){
			System.out.println(counter);
		}
	}
}
```

### While Loop

![alt text](https://github.com/ChenaLee/GWC_UMN_Intro_Java_Curriculum/blob/master/images/While_Loop.png "While Loop Diagram")

While loop is actually very similar to for loop, and the main difference is in how they look. Please compare the diagrams in our For Loop section with the diagram in this session. Can you spot the differences and how our while loop would work?

Let's run through how the code flow:

1. We first initalize our counter outside of our while loop.
2. Then we look to see if our condition fail or not. If it doesn't we continue to our statments.
3. We run our statements.
4. We then modify our variable using the modifier.
5. Now we check if our condition fail or not again. 
	* If it fail then we skip our statements and our for loop end
	* if it doesn't fail we go to our statements and continue with our loop.


#### Exercise 1: Practice with While Loop
For this exercise, your job will be to recreate the for loop we have in exercise 0 as a while loop. The code below should provide you with a good starting point, fill out the `...` with the appropriate code.

```
package GwcS2019Chena;

public class Loops {
	public static void main(String[] args) {
		int counter = ...;
		while(...) {
			...;
			...;
		}
	}
}
```

Hint: If you are stuck, identify the components in the for loop and see where you can place them in the while loop.

#### Exercise 2: Sum with loops

Let's say we want to add every number between 0 and 15 and we want to write this as a loop, how would we do it ? What would we need ? Your task is to write a for loop / while loop that will do this.

```
package GwcS2019Chena;

public class Loops {
	public static void main(String[] args) {
		int sum = 0;
		# Your code goes here
		System.out.println(sum);
	}
}
```
Some hints for you:  

1. Work through each of the components, what do you want each of them to do ?
2. For loop or while loop ? (Both works but which one is easier for you ?)
3. Try to go through how you would add every number from 0 to 15, step by step. See how you can apply this to a loop.

Extra: If you wrote your answer with a for loop, try with a while loop and vice versa.

#### Exercise 3: Fibonacci Number

Fibonacci Number is a specifc sequence of number that goes like this:  

`
0, 1, 1, 2, 3, 5, 8, 13, 21, ....
`

Can you see the pattern ?

Every number in a fibonacci sequence is determined by the sum of the last two number before it, and we start of with 0 and 1 as our first two numbers.

What does this have to do with loops ?

Well it is pretty obvious right ? Your task is to write a block of code that will print a specific length of fibonacci number sequences.

This block of code should get you started. 

```
package GwcS2019Chena;

public class Loops {
	public static void main(String[] args) {
		
		# Setting up some variables that would be very useful to you
		int first_number = 0;
		int second_number = 1;
		
		# Modify this variable to the length that you would like your sequence to be
		int length_of_sequence = 6;
		
		# Your code goes here, good luck.
	}
}
```

If we are to run your completed code with `length_of_sequence` as 6, we should get: 

```
0
1
1
2
3
5
```

As with previous questions, if you have written your loop in one structure, try the other!

#### Exercise 4: Loops within Loops - Pattern Creation !!!

This will be quite a challenging task but we will help you out as much as we can.

Now that we can confidently write a loop structure, it is time to put one loop in another loop.

This can be quite complicated to think about and we really suggest you take your time to work through an example on paper to see how your code should be running.

This is your task, to create a right angle triangle like the example given to you at the beginning. However there will be a twist, your triangle should look like this:

```
1
1 2
1 2 3
1 2 3 4
1 2 3 4 5
```

We will provide you with all the information and tips you need to create this but you will be writing the looping structures.

```
package GwcS2019Chena;

class Loops {
   public static void main(String[] args) {
      
      # How many rows do you want your triangle to have ?
      int rows = 5;
      
      # Your code here
   }
}
```

Some extra tips to help you (You should definetely read this):

You guys have learn that `System.out.println("....")` will print a new line for you. However there is a simplier printing function that will print out something new on the same line for you: `System.out.print("....")`

An example:  

```
System.out.println("Hello");
System.out.println("My");
System.out.println("World");

# These three lines will print out

Hello
My 
World

System.out.print("Hello ");
System.out.print("My ");
System.out.print("World ");

# These three lines will print out

Hello My World

```

If you are really stuck, refer to this block of code shown at the beginning:

```
for (int row = 0; row <= 7; row++){
	String line = '';
	for (int col = 0; col < row; col++) {
		line = line + " #";
	}
	System.out.println(line);
}

```
Output:

```
#
# #
# # #
# # # #
# # # # #
# # # # # #
# # # # # # #
```

Good Luck !!!


 



