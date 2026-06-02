## Ex-6:Python OOP: Abstract Class & Method Example

## Aim:
To create an abstract class named Shape with an abstract method calculate_area, and implement this method in two subclasses: Rectangle and Circle.

## Algorithm:
1. Import ABC module:
    Use from abc import ABC, abstractmethod to define abstract classes and methods.
2. Create Abstract Class Shape:
    Define an abstract method calculate_area() with @abstractmethod.
3. Create Subclass Rectangle:
    Set default values for length and breadth.
    Override calculate_area() to compute the rectangle area.
4. Create Subclass Circle:
    Set default value for radius.
    Override calculate_area() to compute the circle area.
5. Create Objects & Call Methods:
   Instantiate Rectangle and Circle.
   Call their calculate_area() methods.
   
## Program:
```
from abc import ABC, abstractmethod

class Animal(ABC):
    @abstractmethod
    def sound(self):
        pass

class Dog(Animal):
    def sound(self):
        print("Bark")

d = Dog()
d.sound()

```
## Output:

<img width="411" height="294" alt="image" src="https://github.com/user-attachments/assets/a8305c0c-57c4-4240-b4aa-5d806f07f69f" />

## Result:
Thus, the Python program for Abstract Class and Abstract Method was executed successfully.

## Ex-5:Python OOP: Encapsulation with Private Members

## Aim:
To implement Encapsulation in Python by defining a class Rectangle with private member variables __length and __breadth.

## Algorithm:
1. Define the Class:
   Create a class Rectangle with two private attributes: __length and __breadth.
2. Initialize Variables:
   Use the __init__() constructor to set initial values for __length and __breadth.
3. Print Values:
   Display the private variables from within the class to demonstrate access.
4. Instantiate the Object:
   Create an object of the Rectangle class to trigger the constructor.
   
## Program:
```
class Student:
    def __init__(self):
        self.__mark = 90

    def display(self):
        print("Mark:", self.__mark)

s = Student()
s.display()
```
## Output:

<img width="425" height="203" alt="image" src="https://github.com/user-attachments/assets/0a286140-c11b-4aba-9974-803def814675" />

## Result:
Thus, the Python program for Encapsulation using Private Members was executed successfully and the private data member was accessed through a class method.






