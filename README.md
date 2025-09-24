Campus Course & Records Manager (CCRM)

CCRM (Campus Course & Records Manager) is a Java-based console application designed to manage student records, courses, enrollments, grades, and backups.
It demonstrates core Java concepts such as Object-Oriented Programming, Design Patterns, Streams, Lambdas, File I/O, and Custom Exceptions.

📌 Features

Student Management

Add, list, and search students by registration number.

Manage student statuses (Active, Inactive, Deceased).

Course Management

Add, list, and search courses by course code.

Associate instructors and departments with courses.

Builder Pattern used for course creation.

Enrollment & Grading

Enroll students in courses with credit limit checks.

Record marks for different assessments.

Auto-compute grades and GPA based on marks.

Generate transcripts for students.

File Operations

Export student and course data to CSV files.

Automated backup system with timestamped directories.

Recursive utility to compute total backup directory size.

Reports

Filter students by status using Java Streams & Lambdas.

Search for courses by instructor name.

Demonstrates usage of Predicate functional interface.

Menu-Driven CLI

Interactive main menu with labeled loops.

Input validation with exception handling.

🛠️ Technologies & Concepts Used

Language: Java (JDK 17+ recommended)

Core Concepts:

Classes, Inheritance, Abstract Classes

Builder Pattern (for Student & Course objects)

Enums with fields & methods

Polymorphism (toString() overrides)

Singleton Design Pattern (AppConfig)

Exception Handling with Custom Exceptions

Streams & Lambdas for filtering and reporting

File I/O with java.nio.file

Try-with-resources and recursion

Bitwise operators and operator precedence

📂 Project Structure
CCRM/
├── CCRM.java              # Main application class
├── students.csv           # Exported student data (generated at runtime)
├── courses.csv            # Exported course data (generated at runtime)
├── ccrm_backups/          # Backup directory (generated at runtime)
└── README.md

🚀 How to Run

Clone the Repository

git clone https://github.com/your-username/ccrm.git
cd ccrm


Compile the Application

javac CCRM.java


Run the Application

java CCRM


Use the menu to manage students, courses, enrollments, and more.

🏗️ Design Highlights

OOP in Practice:
Classes such as Student, Instructor, Course, and Enrollment model real-world entities.
Person is an abstract class demonstrating inheritance and abstraction.

Builder Pattern:
Used for constructing Student and Course objects cleanly.

Singleton Pattern:
AppConfig ensures that configuration data is loaded only once.

Custom Exceptions:
DuplicateEnrollmentException and MaxCreditLimitExceededException handle business logic errors gracefully.

Functional Programming:
Streams and lambdas are used to filter students and courses dynamically.

🗄️ Data Persistence

Export: Student and course data are exported as CSV files for persistence.

Backup: Automated timestamped backups are created in the ccrm_backups directory.

📌 Future Enhancements

Add database integration (MySQL, PostgreSQL) for permanent storage.

Implement a GUI or web-based interface.

Support for importing data from CSV.

Add role-based access control for admin/teacher users.
