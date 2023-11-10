

> Tasks to complete:

- [x] Research program structure methods and options
- [x] Compare options to find the one which is most appliable
- [x] Give notes on limitations

***

# Understanding the brief

**Programming Language Options (according to the brief):**
* Java
* Python

The project involves creating a timetabling system. To do this, a `dedicated algorithm` must be designed for this purpose that can` avoid clashes of timeslots and rooms` and assigning `appropriate classrooms and number of slots/contact hours` to the `courses and teacher/lecturer names`. There are multiple parts that need to be considered when discussing a software project such as this one:

> Object-oriented Programming

It naturally makes sense to use Object Oriented Programming concepts to create this system. Each layer of the timetable system has its own individual parameters that need to be considered, and therefore multiple objects can be used for this.

For example, there is a main timetabling object which consists of Classroom objects. Classroom objects then contain Week objects, which contain Day objects, which contain Timeslot objects.

	Timetable Obj --> Classroom Obj --> Week Obj --> Day Obj --> Timeslot Obj

> Composite pattern design

This application must have a composite configuration design, which lets the timetable include or uproot numerous scheduled classes. It is an object-oriented concept, which describes a group of objects that are treated the same way as a single instance of the same type of object. https://en.wikipedia.org/wiki/Composite_pattern. It is similar to a tree-like structure.

Here is an example of this design being used:
https://www.digitalocean.com/community/tutorials/composite-design-pattern-in-java

``` Java
package com.journaldev.design.composite;

import java.util.ArrayList;
import java.util.List;

public class Drawing implements Shape{

	//collection of Shapes
	private List<Shape> shapes = new ArrayList<Shape>();
	
	@Override
	public void draw(String fillColor) {
		for(Shape sh : shapes)
		{
			sh.draw(fillColor);
		}
	}
	
	//adding shape to drawing
	public void add(Shape s){
		this.shapes.add(s);
	}
	
	//removing shape from drawing
	public void remove(Shape s){
		shapes.remove(s);
	}
	
	//removing all the shapes
	public void clear(){
		System.out.println("Clearing all the shapes from drawing");
		this.shapes.clear();
	}
}
```


---

# Option Analysis

>Analysis of Options:

To construct the most efficient program that we can achieve, we need to use tools that will empower the use of these object-oriented concepts and adhere to the brief as much as possible.

Two options are already proposed in the brief: using either Python or Java to implement the software application. To decide, various factors are considered:

> First Option Analysis: which programming language?

* `Python` supports object-oriented programming and is simple and easy to learn, but has a lot `more work involved and unusual code syntax with implementing OOP`. It was not designed wholly with object-oriented systems in mind unlike Java, and our team has less experience with Python.

* `Java` on the other hand, has a much more `linear and pre-prepared syntax for object-oriented programming` than Python. It suits the purposes of our application much better naturally. Java is also `statically typed`, meaning compiled before execution, making it `faster than Python`, which is a `dynamically typed language`. Our team also has two members that have experience in Java (have modules with Java as the programming language) and have more ideas on how to design the program.

> Second Option Analysis: PRESENTATION FORMAT

---

	 Complexity: How complex is the development and maintenance of each option?

* Python: Simple, easy to use, easy to understand. +

* Java: Similar to C++, more complex, more robust. -

---

	`Customization: To what extent can each option be tailored to the specific requirements`

* Python: Customizable, but not created with OOP in mind. Possible difficulties with adhering to requirements -

* Java: Built with OOP in mind. Very customizable in reference to OOP concepts such as composite pattern design and management of multiple objects. +

---

	`Scalability: How well does each option accommodate future growth and changes?`

* Python: Interpreted language and slower than Java. Not built with OOP in mind: more structure required to design the application to suit the concepts utilised and scale. -

* Java: Compiled language and therefore faster. With OOP, very easy to scale to larger software designs and maintain security and high speed. Naturally easy to have communication between different files. +

---

	`Risk: What are the potential risks and uncertainties assiocated with each problem`

 * Python: Risks of complications, sloppier syntax when using OOP, and harder to debug. Only one member has knowledge of this language. -
 
 * Java: Highly disciplined syntax and understandable with OOP. Easier to debug. Less risk involved. Two members in the team regularly use Java. +






