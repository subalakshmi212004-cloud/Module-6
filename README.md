README
🐍 Python OOP: Abstract Class & Method Example
🎯 AIM
```
To create an abstract class named Shape with an abstract method calculate_area, and implement this method in two subclasses: Rectangle and Circle.
```
🧠 ALGORITHM
``
1.Import ABC module:

   Use from abc import ABC, abstractmethod to define abstract classes and methods.
2.Create Abstract Class Shape:

   Define an abstract method calculate_area() with @abstractmethod.
3.Create Subclass Rectangle:

   *Set default values for length and breadth.
   *Override calculate_area() to compute the rectangle area.
4.Create Subclass Circle:

  *Set default value for radius.
  *Override calculate_area() to compute the circle area.
5.Create Objects & Call Methods:

   *Instantiate Rectangle and Circle.
   *Call their calculate_area() methods.
💻 Program
```
from abc import ABC, abstractmethod
import math
class Shape(ABC):
    @abstractmethod
    def calculate_area(self):
        pass
class Rectangle(Shape):
    def __init__(self, length=1, breadth=1):
        self.length = length
        self.breadth = breadth

    def calculate_area(self):
        return self.length * self.breadth
class Circle(Shape):
    def __init__(self, radius=1):
        self.radius = radius

    def calculate_area(self):
        return math.pi * self.radius *self radius
rect = Rectangle(5, 3)
circle = Circle(4)

print("Area of Rectangle:", rect.calculate_area())
print("Area of Circle:", circle.calculate_area())
```
Output
<img width="858" height="181" alt="530075337-7f3a2943-6112-464e-bbeb-5d639b3892c5" src="https://github.com/user-attachments/assets/70e1ac0b-efdd-44e4-b505-5e6e47bbf463" />


Result
Thus , the program has been executed succesfully.

🐍 Python OOP: Encapsulation with Private Members
🎯 AIM
```
To implement Encapsulation in Python by defining a class Rectangle with private member variables __length and __breadth.
```
🧠 ALGORITHM
```
Define the Class:

Create a class Rectangle with two private attributes: __length and __breadth.
Initialize Variables:

Use the __init__() constructor to set initial values for __length and __breadth.
Print Values:

Display the private variables from within the class to demonstrate access.
Instantiate the Object:

Create an object of the Rectangle class to trigger the constructor.
💻 Program
```class Rectangle:
    def __init__(self, length, width):
        # private variables
        self.__length = length
        self.__width = width

    def display(self):
        # accessing private variables within the class
        print(self.__length)
        print(self.__width)

# create object
rect = Rectangle(5, 3)

# print values within the class
rect.display()
```
Output
<img width="740" height="186" alt="530075472-e7d44b0a-cdaf-49dd-b07c-2b4b42058262" src="https://github.com/user-attachments/assets/74cebce3-a35b-443c-8e22-51a49ab9dac2" />


Result
Thus , the program has been executed succesfully.

🐟 Method Overriding-Fish and Shark Class Inheritance in Python
🧠 AIM:
```
To write a Python program that demonstrates class inheritance by creating a parent class Fish with a method type, and a child class Shark that overrides the type method.
```
📋 ALGORITHM:
```
Define the Fish class with a method named type() that prints "fish".
Define the Shark class as a subclass of Fish, and override the type() method to print "shark".
Create an instance of the Fish class named obj_goldfish.
Create an instance of the Shark class named obj_hammerhead.
Use a for loop to iterate over both objects.
Within the loop, call the type() method using the loop variable.
Output will demonstrate method overriding: printing "fish" and "shark" accordingly.
```
💻 PROGRAM:
```
class Fish:
    def type(self):
        print("fish")
class Shark:
    def type(self):
        print("shark")
obj_goldfish=Fish()
obj_hammerhead=Shark()

for i in (obj_goldfish,obj_hammerhead):
    i.type()
```
OUTPUT
<img width="746" height="180" alt="530075596-0253ad6d-ce4b-4b4e-9ea0-97aa087020c5" src="https://github.com/user-attachments/assets/5537fa2b-c03f-44da-b423-57cc817b9323" />


RESULT
Thus , the program has been executed succesfully.

🐍 Python OOP: Operator Overloading (Less Than <)
🎯 AIM
```
To write a Python program that demonstrates operator overloading by overloading the less than (<) operator using a custom class.
```
🧠 ALGORITHM
```
Create Class A:

Define the __init__() method to initialize the object with a value a.
Overload the < Operator:

Define the __lt__() method with logic:
If self.a < o.a, return "ob1 is less than ob2"
Else, return "ob2 is less than ob1"
Create Objects:

Instantiate two objects ob1 and ob2 with values.
Use < Operator:

Use print(ob1 < ob2) to trigger the overloaded behavior.
```
💻 Program
```
class A:
    def __init__(self, a):
        self.a = a
    def __lt__(self, other):
        if(self.a<other.a):
            return "ob1 is less than ob2"
        else:
            return "ob2 is less than ob1"
ob1 = A(20)
ob2 = A(3)
print(ob1 < ob2)
```
Output
<img width="944" height="170" alt="530075722-161de29c-1da7-440f-b52c-30c03bc69a51" src="https://github.com/user-attachments/assets/559a468a-baf0-4490-bec0-d2a2e464a6e0" />

Result
Thus , the program has been executed succesfully.

# 🐍 Python OOP: Polymorphism with Classes
🎯 AIM
```
To create two specific classes — Beans and Mango. Then, create a generic function that can accept any object and determine its type (Fruit or Vegetable) and color, using polymorphism.
```
🧠 ALGORITHM
```
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
```
💻 Program
```
class Beans(): 
     def type(self): 
       print("Vegetable") 
     def color(self):
       print("Green") 
class Mango(): 
     def type(self): 
       print("Fruit") 
     def color(self): 
       print("Yellow")      

obj_beans = Beans() 
obj_mango = Mango() 
for i in (obj_beans,obj_mango):
    i.type()
    i.color()
```
Output
<img width="945" height="231" alt="530075842-2db089d6-e0d9-4c13-a1a1-8f678f41398c" src="https://github.com/user-attachments/assets/19dc132e-3a51-4217-b436-6471e2b7b050" />


Result
Thus , the program has been executed succesfully.

