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

## Ex-6:Python OOP: Encapsulation with Private Members

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

## Ex-6:Method Overriding-Fish and Shark Class Inheritance in Python

##  AIM:
To write a Python program that demonstrates class inheritance by creating a parent class Fish with a method type, and a child class Shark that overrides the type method.

## ALGORITHM:

1.Define the Fish class with a method named type() that prints "fish".
2.Define the Shark class as a subclass of Fish, and override the type() method to print "shark".
3.Create an instance of the Fish class named obj_goldfish.
4.Create an instance of the Shark class named obj_hammerhead.
5.Use a for loop to iterate over both objects.
6.Within the loop, call the type() method using the loop variable.
7.Output will demonstrate method overriding: printing "fish" and "shark" accordingly.

## PROGRAM:
```
class Fish:
    def swim(self):
        print("Fish can swim")

class Shark(Fish):
    def swim(self):
        print("Shark swims fast")

s = Shark()
s.swim()
```
## OUTPUT:

<img width="399" height="228" alt="image" src="https://github.com/user-attachments/assets/0e6c2402-b698-4336-8c82-878991f9005e" />

## RESULT:
Thus, the Python program for Method Overriding using Fish and Shark class inheritance was executed successfully.

## Ex-6:Python OOP: Operator Overloading (Less Than <)

##  Aim:
To write a Python program to demonstrate Operator Overloading using the Less Than (<) operator.

## Algorithm:

1.Define a class Number.
2.Create a constructor to initialize the value.
3.Overload the __lt__() method to compare two objects.
4.Create two objects with different values.
5.Compare the objects using the < operator.
6.Display the result.
7.End the program.

## Program:
```
class Number:
    def __init__(self, value):
        self.value = value

    def __lt__(self, other):
        return self.value < other.value

n1 = Number(10)
n2 = Number(20)

print(n1 < n2)

```
## Output:

<img width="435" height="237" alt="image" src="https://github.com/user-attachments/assets/53979544-fb13-48fe-a9bd-b61ec99b3e14" />

## Result:
Thus, the Python program for Operator Overloading using the Less Than (<) operator was executed successfully.

## Ex-6:Python OOP: Polymorphism with Classes

## Aim:
To write a Python program to demonstrate Polymorphism using classes.

## Algorithm:

1.Define a class Dog with a method sound().
2.Define a class Cat with a method sound().
3.Create a function make_sound() that calls the sound() method.
4.Create objects of Dog and Cat.
5.Pass the objects to the make_sound() function.
6.Display the respective sounds.
7.End the program.

## Program:
```
class Dog:
    def sound(self):
        print("Bark")

class Cat:
    def sound(self):
        print("Meow")

def make_sound(animal):
    animal.sound()

d = Dog()
c = Cat()

make_sound(d)
make_sound(c)

```
## Output:

<img width="402" height="339" alt="image" src="https://github.com/user-attachments/assets/6c998c6c-4bd4-4e0e-9e92-ac2af841cd85" />

## Result:
Thus, the Python program for Polymorphism with Classes was executed successfully and different objects responded to the same method call in their own way.
