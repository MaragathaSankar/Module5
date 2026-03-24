# Multilevel Inheritance Example in Python

This Python project demonstrates the concept of **Multilevel Inheritance** to collect and display the **name**, **age**, and **location** of a person.

## 🎯 Aim

To write a Python program that uses multilevel inheritance to get and display a person’s name, age, and location.

## 🧠 Algorithm

1. **Parent Class**  
   - `__init__(name)` initializes the `name` attribute.  
   - `getName()` returns the `name`.

2. **Child Class (inherits Parent)**  
   - `__init__(name, age)` initializes `name` using `super()` and adds `age`.  
   - `getAge()` returns the `age`.

3. **Grandchild Class (inherits Child)**  
   - `__init__(name, age, location)` initializes `name` and `age` using `super()` and adds `location`.  
   - `getLocation()` returns the `location`.

4. **Input & Output**  
   - Take user input for name, age, and location.  
   - Create an instance of `Grandchild`.  
   - Print all details using class methods.

## Program
```python
class Person:
    def __init__(self, name):
        self.name = name

    def getName(self):
        return self.name


class Age(Person):
    def __init__(self, name, age):
        super().__init__(name)
        self.age = age

    def getAge(self):
        return self.age


class Location(Age):
    def __init__(self, name, age, location):
        super().__init__(name, age)
        self.location = location

    def getLocation(self):
        return self.location


name = input("Enter Name: ")
age = int(input("Enter Age: "))
location = input("Enter Location: ")


person1 = Location(name, age, location)



print("Name:", person1.getName())
print("Age:", person1.getAge())
print("Location:", person1.getLocation())

```
## Sample Output
<img width="584" height="181" alt="image" src="https://github.com/user-attachments/assets/f59e1195-c99d-4bed-82b6-f0c472869288" />

## Result
The program successfully demonstrates Multilevel Inheritance in Python by collecting and displaying a person’s name, age, and location using three classes.

