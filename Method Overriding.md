# 🐟 Method Overriding-Fish and Shark Class Inheritance in Python

## 🧠 AIM:
To write a Python program that demonstrates class inheritance by creating a parent class `Fish` with a method `type`, and a child class `Shark` that overrides the `type` method.

## 📋 ALGORITHM:

1. Define the `Fish` class with a method named `type()` that prints `"fish"`.
2. Define the `Shark` class as a subclass of `Fish`, and override the `type()` method to print `"shark"`.
3. Create an instance of the `Fish` class named `obj_goldfish`.
4. Create an instance of the `Shark` class named `obj_hammerhead`.
5. Use a `for` loop to iterate over both objects.
6. Within the loop, call the `type()` method using the loop variable.
7. Output will demonstrate method overriding: printing `"fish"` and `"shark"` accordingly.

## 💻 PROGRAM:
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
## OUTPUT
<img width="746" height="180" alt="530075596-0253ad6d-ce4b-4b4e-9ea0-97aa087020c5" src="https://github.com/user-attachments/assets/ad697756-e41d-4c92-bf5a-35c26a600b6a" />

## RESULT
Thus , the program has been executed succesfully.



