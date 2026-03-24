# # Constructors in Python: Welcome Message with Student Name

## 🎯 Aim
To write a Python program that creates a **Student** class with a **default constructor** and a method to display a welcome message along with the student’s name provided by the user.

## 🧠 Algorithm
1. **Get user input**: Accept the student's name from the user.
2. **Define the class**: Create a class `Student` with a default constructor (`__init__`).
3. **Default Constructor**: In the constructor, assign the user input (student name) to an instance variable `self.a`.
4. **Display Message**: Define a method `show` that prints "This is non-parameterized constructor" and a welcome message with the student’s name.
5. **Execute the Program**: Instantiate the `Student` class and call the `show` method.

## 🧾 Program
```python
class Student:
    def __init__(self):
        self.a = input("Enter Student Name: ")

    def show(self):
        print("This is non-parameterized constructor")
        print("Welcome,", self.a)
s1 = Student()
s1.show()
```
## Output
<img width="838" height="220" alt="image" src="https://github.com/user-attachments/assets/45adc714-ae27-4e3a-bb64-85338bbb11c5" />


## Result
The program successfully demonstrates the use of a default constructor in Python by taking a student’s name as input and displaying a welcome message along with the constructor message.
