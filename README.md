# DV1537_OOP_CPP
DV1537 Object-Oriented C++ Course




## General instructions

1. Use GIT version control to manage your code and submit assignments unless specified otherwise (see separate instructions on how to set up and use GIT Classroom)
2. Your program should use files as the only input. No keyboard input is permitted.
3. Format output exactly as specified/exemplified in the assignment descriptions
3. Follow good code writing practices:
	a. Do not use global variables
	b. Divide classes into .cpp and .h files
	c. All parameters that are constants should be declared as such
	d. All variable and class names should be in English, self-explanatory, and must use CamelCase. 
	e. All code that is not used should be removed
	f. Use code comments when the reasoning behind the solution is not obvious
	g. Always check that that all allocated memory is released and avoid memory leaks
4. You should not use any external libraries other than `math`, `iostream`, and `fstream`. 



## Assignment A

The aim of assignment A is to test your understanding on pointers and working with classes. The focus
is on memory management, class inheritance, encapsulation, and overloading. This assignment has 4 deliverables:

### A1: Pointers and memory management

#### Instructions:
	- Write a program that reads numbers from a file into a buffer. 
	- When the end of the file is reached, the program outputs all numbers that are above the average
	- You must store the numbers in a dynamic array and extend the length of the array as needed.

#### Example:
```
	Input: 1 2 3 4 5		Output: 4 5
	Input: 0 0 0 0 1		Output: 1
	Input: 1 1			Output: <nothing is printed> 
```

### A2: Classes
	Instructions:
		- Implement an abstract class Shape with methods:
			- getType() returns a string denoting type of a shape (point, line, polygon ..)
			- area() returns area of the object, or 0 if the shape is concave or intersecting
			- circumreference() returns circumreference of the object
			- position() returns center coordinates of the object
			- isConvex() returns true if shape is convex
			- distance(Shape s) returns distance to the center of another shape
		- Extend the Object classe into Point, Line, Triangle, and Polygon. Overload the inherited methods. Constructors of these classes take vertices coordinates as an input

HOW TO TEST THIS???? How to provide input via file


A3: Operator overloading & object cloning
	Instructions:
		- Overload the assignment operator (=) that deep copies the object. 
		- Overload the addition operator (+) that makes possible to add more points to a polygon. The added points extend the polygon
		- Overload the << operator to print a shape.
		
HOW TO TEST THIS???? How to provide input via file


A4: Class diagrams
	Instructions:
		- Draw a class diagram illustrating the class structure of A1-A3. Follow UML class diagram notation. Introduce and describe the figure.
		- Describe 3 benefits of OOP over procedural programming.
		- Describe 3 disadvantages of OOP over procedural programming. 
		- Motivate your answers with examples and references to credible online sources.
		- Total length of the report should not exceed 2 pages.


Assignment B
------------
This assignment builds upon the previous assignment and introduces sorting algorithms, and recursion, in the context of 
object-oriented programming. This assignment has 3 deliverables:


B1: Polymorphism
	Instructions:
		- Implement a Figure class enabling grouping of shapes. The Figure class should have the following methods:
			- addShape(Shape s) adds a shape to the group
			- getBoundingBox() calculates the minimum axis-aligned bounding rectangle to fit all the figures. The method returns top left and bottom right corners of the box.
			
B2: Recursion
	Instructions:
		- Extend the Figure class with the following:
			- getClosest(Shape location, int s, int n) - orders the list of shapes by their distance from the location and returns n closest shapes starting from s.
			- In the class, you must implement a recursive sorting algorithm of your choice


B3: Class diagrams
	Instructions:
		- Extend the class diagram from A4 with the new classes/methods.
		- When to use and when not to use recursion
		- Compare 3 sorting algoritms by ( no O measure)

