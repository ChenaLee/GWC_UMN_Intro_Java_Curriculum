# 06_Function_Arguments_and_Data_Structure_Basic
## Function Arguments
Let's go back to the factory example.  
When worker A does their job and the worker B does the next step, A might pass B something. In our example, it would be a teddy bear in progress.  
  
To do this in programming, we use **function arguments**. They are something you can pass to a function. In other words, a function can take function arguments.  

You've seen something like this and coded inside of this block before :
```
public static void main(String[] args) {
  int number = 1;
	System.out.println(number);
}
```
The **args** in the bracket next to "main" is a function argument. **String[]** is a type. To specify what kind of arguments a function can take like this, put brackets next to the function name, and put data type and name of the argument. To make a function with multiple arguments, put a comma in between arguments like this:  
```
void myFunction(int number, String name) {
	...
}
```
Take a look at **println** again as well. It has a bracket that contains **number**. This is how you call a function with function arguments, or "pass" the function some variables.  


- 1 argument
- 2 arguments
- 2 arguments, but you wanna only pass one of it? Try calling
- functions with same name but different arguments
- Collection types data structures

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
