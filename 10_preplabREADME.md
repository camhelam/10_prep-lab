# 10_prep-lab

10.9 Prep Lab: Polymorphic class list

You are teaching a class which contains a mix of undergraduate students and graduate students. Undergraduate students are objects of the class Student. Graduate students are objects of the class GradStudent which is derived from the class Student. In your class you want to keep both types of students in a single list (a vector) without having to worry about which specific type the student is. GradStudents are Students but they have the additional data member of researchArea.

Your program will loop asking for one of three options (add, print, or quit).

Add user option: You will create (using new) a Student object or a GradStudent object and add its pointer to the vector classMembers.

Print user option: You will print the entire class last, using the appropriate ToStr member function. You should not test whether a particular pointer in the class list points to a Student or a GradStudent. The correct ToStr function will be called automatically if you have properly defined functions for ToStr.

We have provided most of the code already for you. You just need to fill in appropriate code at the locations marked with comments.

Note: In Student the name data member is declared as protected. We usually declare it is private meaning only member functions of Student could directly access name and all other functions would need to use an accessor function from Student to get access to that data. When declared as protected, that means it is also directly accessible by member functions in derived classes, but invisible to all other functions.

Here is an example of what a run would look like:

Option: add
Name: Mary
If grad student enter a one word research area, else enter "NO": MachineLearning

Option: add
Name: Bob
If grad student enter a one word research area, else enter "NO": NO

Option: print
Mary is a graduate student researching the area of MachineLearning.
Bob is an undergraduate student.

Option: quit
