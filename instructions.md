##  Instructions

Student Grade Book Project - 

Step 1: Classes
The first thing we need is a way to represent a "student" in our program. This is where classes come in handy! A class is like a 
blueprint for creating objects. Our Student class will define what characteristics (attributes) a student has and what actions 
(methods/functions) a student can perform.

Your Task:

    1. Define the Student Class:

        * Create a class named Student.

    2. Inside the class, define an __init__ method. This is a special method that gets called automatically when you create a new Student object.

        * The __init__ method should take self, name, and student_id as parameters.

        * self refers to the instance of the class being created.

        * name will be the student's name (e.g., "Alice Smith").

        * student_id will be a unique identifier for the student (e.g., 101).

    3. Inside __init__, you'll assign these parameters to instance variables:

        * self.name = name

        * self.student_id = student_id

    4. Also, initialize an empty dictionary within the __init__ method to store the student's grades. Let's call it self.grades. 
    This dictionary will map subject names (strings) to their scores (integers or floats). For example: {"Math": 90, "Science": 85}.

    5. Finally, initialize an empty set within the __init__ method to keep track of all unique subjects a student is enrolled in. Let's call it self.subjects_enrolled.


### Here's a skeleton to get you started:

class Student:
    def __init__(self, name, student_id):
        # Assign name and student_id to instance variables
        # Initialize self.grades as an empty dictionary
        # Initialize self.subjects_enrolled as an empty set

#### Why are we using these concepts here?

    * Classes (Student): To create a structured way to store all the information related to a single student (their name, ID, and grades) as one cohesive unit.

    * __init__ method: This is the constructor. It sets up the initial state of every new Student object you create.

    * Dictionary (self.grades): Perfect for storing key-value pairs. Here, the subject name is the key, and the grade is the value. 
    This allows for easy lookup and modification of grades by subject.

    * Set (self.subjects_enrolled): A set is ideal for storing unique items. We'll use it to ensure we only store each subject once, 
    even if a student gets multiple grades in the same subject over time.
