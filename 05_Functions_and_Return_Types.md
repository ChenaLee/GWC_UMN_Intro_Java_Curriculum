# 05_Functions_and_Return_Types
## Function
A function is like an individual in a factory that does one specific job.  
For example, worker A's job might be connecting teddy bear's head and body together, 
worker B's job might be putting eyes on the teddy bear after worker A, 
and worker C might be the one finishing it buy drawing its mouth.  
  
In programming, functions can call other functions to complete a job as well.  
Function A might call function C, and function B can use function C too.

Making functions with one specific job each instead of putting all the code in one function provides the benefic of reusability.  
    Let's say you made a function to find an average of 2 numbers. 
    When you try to make another function that finds average of all test scores of your class, 
    it could call the average function you already made.  
    You could later also want to implement a function that finds average of all test scores of one person, the average function could be used again.  
    As a function gets more complicated, this will reduce the amount of code you write and dupulicate code you have to maintain significantly.  

You've seen something like this and coded inside of this block before :
```
public static void main(String[] args) {
  int number = 1;
	System.out.println(number);
}
```
This is called the "main function". Main function runs every time you "run a program". In other words, no other function is automatically called when you "run a program".  
That means main has to call other functions if you want other functions to run.  
The "println" you've used is also a function. It ran because the main function called it.  There are many functions created by experts and available to you like the print. You can use them or create your own functions when you need.  

## Function Name
```
public int myFunction() {
   ...
}
```
This is an example of functions. Each function has a name. For this one, "myFunction" is the name of the function.

## Return
Just like that math function f(x) = 1 always give you 1, a function can give a **return** when it's called.  
  
```
public int myFunction() {
   return 0;
}
```
This means the function **exits** at this point and gives back the number 0 to the function that called this function.
  
  
```
public int myFunction() {
  return 0;
  System.out.println("This is never printed");
}
```
As function exits when it hits the "return" line, the println line will never execute.
  
  
```
public int myFunction() {
  if (false) {
    return 0;
  }
  System.out.println("This is always printed");
  return 1;
}
```
However, this println will always execute because nothing no "return" was hit before it reaches the println.  
  
  
## Return Types of Functions
1. **void**
  This means it returns nothing.
  ```
  public void printMyInformation() {
      ...
  }
  ```
2. Any other variable types  
  ```
  public void printMyInformation() {
      ...
  }
  
  public String getMyName() {
      ...
  }
  
  public int getMyAge() {
      ...
  }
  ```
  
## Calling a Function
```
public void myFunction() {
		yourFunction();
}
```
This is the simplest function call. myFunction is calling yourFunction.  
  
However, what if yourFunction's job was to return an integer and myFunction has to use the integer?  
```
public void myFunction() {
		int value = yourFunction();
}
```
This saves the integer returned by yourFunction into the integer variable with the name "value".  

## Exercises
### Exercise 0 : Void function that prints
Create a function with:
- Name : printHello  
- Return Type : None (void)  
- Job : Print "Hello"  

And let the main function call it.

### Exercise 1 : Calling a function.
Create a function with:
- Name : getMyName  
- Return Type : String   
- Job : return String that has your first name as its value   
  
Create a function with:
- Name : getMyAge  
- Return Type : int  
- Job : return int that has your age as its value    
  
Create a function with:
- Name : printMyInfo  
- Return Type : None (void)    
- Job : Print "{Your Name} is {Your Age} years old." Get your name and your age by calling getMyName and getMyAge functions.  
  
And let the main function call printMyInfo.

### Exercise 2 : Reuse a function
Create a function with:
- Name : getFriendName  
- Return Type : String   
- Job : return String that has your friend or family's first name as its value   
  
Create a function with:
- Name : getFriendAge  
- Return Type : int  
- Job : return int that has your friend or family's age as its value    

Create a function with:
- Name : printAgeDifference  
- Return Type : None (void)    
- Job : Print "{Your Name} and {Friend Name} have {Age Difference} years old." Get your name and your age by calling getMyName and getMyAge functions. Get your friend's name and age by calling getFriendName and getFriendAge.  
Note that you are reusing getYourName and getYourAge that you've previously created. How convenient!
  
Let the main function call printAgeDifference.
