Student Management System Documentation
Overview:
This C++ program implements a Student Management System using templates and vectors. It allows users to:

Add new students
Display all students
Remove a student by ID
Search for a student by ID
Exit the program

The program follows an object-oriented approach, utilizing class inheritance to manage students effectively.

Class Structure
1. Student<T> (Base Class)
This is a template class that stores student information. It contains:
Attributes:
vector<T> id: Stores student IDs
vector<T> name: Stores student names
Constructor: Displays an initialization message
Destructor: Displays a message when the object is destroyed.

2. StudentManagement<T> (Derived Class)
This class inherits from Student<T> and provides four functionalities:
Adding Students (addStudent())
Displaying Students (displayAllStudents())
Removing Students by ID (removeStudentById())
Searching Students by ID (searchStudentById())
Function Descriptions:

addStudent()
Takes user input for student ID and name.
Uses vector.push_back() to store them.

displayAllStudents()
Displays all student IDs and names.
Checks if the student list is empty before displaying.

removeStudentById()
Searches for a student by ID.
If found, removes the student using vector.erase().
If not found, displays an error message.

searchStudentById()
Searches for a student by ID.
If found, displays their details.
If not found, shows an error message.

3. main() Function
The main function presents a menu-driven interface where users can choose operations.
Functionalities:
Loop Until Exit (do-while loop)
Menu Display (switch-case for user selection)
Calls the Appropriate Functions



