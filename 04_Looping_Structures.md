# 04_Looping_Structures

## Looping in Java

A loop in programming language is a way of writing code in such a way that allow us to run a block of code in a finite and determined amount of time. 

An example of this would be that you would be that we want to draw a right-angle triangle made out of "#" on our console. 

#
# #
# # #
# # # #
# # # # #
# # # # # #
# # # # # # #

One way to do this is to write seven lines of:

System.out.println("#");
System.out.println("# #");
System.out.println("# # #");
System.out.println("# # # #");
System.out.println("# # # # #");
System.out.println("# # # # # #");
System.out.println("# # # # # # #");

This is very inefficient and tedious and we would like to write some code that is both smarter, easier to read, and more efficient.

Here's an example of something we can write and by the end of the class you can write one yourself as well. (If you don't know what String is and how they work, go here ....)

for (int row = 0; row <= 7; row++){
	String line = '';
	for (int col = 0; col < row; col++) {
		line = line + " #";
	}
	System.out.println(line);
}

## Structures / Components

Loop structures are the name we give to different variantion of loops that we can write and each of them will work in a sightly different manner but the same concept still apply, we are trying to run a group of code multiple times.

Now we will explain each of the components that comes into making a loop:
Counter - A variable that we use to help us manage our loop.
Initialization - Use to create our counter and giving it a value.
Loop-condition - Use to determine whether we should continue with the loop or terminate it base on our counter.
Modifiers - What we do to our counter every loop.
Statments(s) - What we want to run every loop.

### For Loop

#### Exercise 0: Practice with For Loop

### While Loop

#### Exercise 1: Practice with While Loop

### Do While

#### Exercise 2: Practice with Do While Loop


