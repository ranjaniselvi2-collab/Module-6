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
Define the Fish class with a method named type() that prints "fish".
Define the Shark class as a subclass of Fish, and override the type() method to print "shark".
Create an instance of the Fish class named obj_goldfish.
Create an instance of the Shark class named obj_hammerhead.
Use a for loop to iterate over both objects.
Within the loop, call the type() method using the loop variable.
Output will demonstrate method overriding: printing "fish" and "shark" accordingly.
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
To write a Python program that demonstrates operator overloading by overloading the less than (<) operator using a custom class.

## Algorithm:
1.Create Class A:

    Define the __init__() method to initialize the object with a value a.

2.Overload the < Operator:

     Define the __lt__() method with logic:
          If self.a < o.a, return "ob1 is less than ob2"
          Else, return "ob2 is less than ob1"
   
3.Create Objects:

    Instantiate two objects ob1 and ob2 with values.

4.Use < Operator:

   Use print(ob1 < ob2) to trigger the overloaded behavior.
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
To create two specific classes — Beans and Mango. Then, create a generic function that can accept any object and determine its type (Fruit or Vegetable) and color, using polymorphism.

## Algorithm:
Create Class Beans:

Define type() method that prints "Vegetable".
Define color() method that prints "Green".
Create Class Mango:

Define type() method that prints "Fruit".
Define color() method that prints "Yellow".
Define Generic Function func(obj):

Call obj.type() and obj.color() — this works with both Beans and Mango objects, showcasing polymorphism.
Create Objects:

Instantiate Beans and Mango.
Pass them to func() and execute the program.
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
