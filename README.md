Download Link: https://assignmentchef.com/product/solved-cs102-lab3-inheritance-abstract-classes-polymorphism
<br>



<ul>

 <li>For all labs in CS 102, your solutions must conform to these <a href="http://www.cs.bilkent.edu.tr/~adayanik/cs101/practicalwork/styleguidelines.htm">CS101/102 style </a><a href="http://www.cs.bilkent.edu.tr/~adayanik/cs101/practicalwork/styleguidelines.htm">guidelines</a>.</li>

 <li>Create a Java Project named Lab03. Put all of your classes in this project.</li>

 <li>Remember to include <strong>javadoc comments </strong>for each class and method.</li>

 <li>Upload your solution <strong>as a single .zip file </strong>to the Lab03 assignment by the end of your section’s lab session in the week of March 1. You must use the following naming convention: Lab03_Surname_FirstName.zip where Surname is your family name and FirstName is your first name. You may upload multiple times; the last upload will be considered.</li>

</ul>

Create an abstract class called <strong>Shape2D</strong>. A 2D shape has two properties: x and y coordinates of its center. Its constructor takes two parameters: x and y coordinates. You may assume that  both coordinates are integers.

This class has the following methods:

<ul>

 <li><strong>public abstract double calculatePerimeter() <em>– </em></strong>returns perimeter of a</li>

</ul>

2D shape. This method will be an abstract method.

<ul>

 <li><strong>public abstract double calculateArea() <em>– </em></strong>returns area of a 2D shape.</li>

</ul>

This method will be an abstract method.

<ul>

 <li><strong>public double calculateDistance( Object anyShape ) – </strong>returns the euclidean distance between the centers of two <strong>Shape2D </strong> If <strong>anyShape </strong>parameter is not a <strong>Shape2D </strong>instance, it should return -1.</li>

 <li><strong>public String toString() – </strong>returns a string representation of two properties: x and y coordinates of its center. Make sure to use <strong>@Override </strong>annotation before the method definition, because this method overrides the <strong>toString() </strong>method in our superclass <strong>Object</strong>.</li>

 <li><strong>public boolean equals( Object o ) – </strong>returns true if given object is a</li>

</ul>

<strong>Shape2D </strong>object that is equal to this one; false otherwise. Make sure to use <strong>@Override </strong>annotation before the method definition, because this method overrides the <strong>equals() </strong>method in our superclass <strong>Object</strong>.

After creating the <strong>Shape2D </strong>class, create the following three classes.

<ul>

 <li>Create a class <strong>Circle </strong>which extends <strong>Shape2D </strong> Circle class has an additional property, <strong>radius</strong>. Circle is a 2D shape, therefore its constructor takes three parameters, x and y coordinates and radius.</li>

 <li>Create a class <strong>Rectangle </strong>which extends <strong>Shape2D </strong> Rectangle class has additional properties, <strong>height </strong>and <strong>width</strong>. Its constructor takes four parameters; x, y coordinates, height and width.</li>

 <li>Create a class <strong>Square </strong>which extends <strong>Shape2D </strong> Square class has an additional property, <strong>sideLength</strong>. Its constructor takes three parameters, x and y coordinates and sideLength.</li>

</ul>

All classes will also implement <strong>calculatePerimeter() </strong>and <strong>calculateArea() </strong>methods, and override <strong>toString() </strong>and <strong>equals() </strong>methods. Reuse the <strong>toString() </strong>and <strong>equals() </strong>implementations in the super class when implementing these methods in the subclasses with <strong>@Override </strong>annotation before the method definitions.

Write a test class, <strong>ShapeTest. </strong>Create <u>an array </u>of three shape objects: one rectangle, one square and one circle. Then, find a 2D Shape object with the longest perimeter and the object with the largest area to the screen and print whether these objects are Square, Circle or Rectangle. You should do this by implementing and using the following methods.

<ul>

 <li><strong>public static Shape2D findLargestArea() <em>– </em></strong>Write a method which takes an array of <strong>Shape2D </strong>objects as parameter and returns the shape with the largest area in the shape list.</li>

 <li><strong>public static Shape2D findLongestPerimeter() <em>– </em></strong>Write a method which takes an array of <strong>Shape2D </strong>objects as a parameter and returns the shape with the longest perimeter in the shape list.</li>

</ul>

Demonstrate the uses of your toString() and equals() methods from these classes. Also, calculate the distances between these three <strong>Shape2D </strong>objects.

<strong>Sample Run</strong>