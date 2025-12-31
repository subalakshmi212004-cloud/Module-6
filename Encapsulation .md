# 🐍 Python OOP: Encapsulation with Private Members

## 🎯 AIM

To implement **Encapsulation** in Python by defining a class `Rectangle` with **private member variables** `__length` and `__breadth`.

---

## 🧠 ALGORITHM

1. **Define the Class**:
   - Create a class `Rectangle` with two private attributes: `__length` and `__breadth`.

2. **Initialize Variables**:
   - Use the `__init__()` constructor to set initial values for `__length` and `__breadth`.

3. **Print Values**:
   - Display the private variables from within the class to demonstrate access.

4. **Instantiate the Object**:
   - Create an object of the `Rectangle` class to trigger the constructor.

---

## 💻 Program
```
class Rectangle:
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

## Output

<img width="740" height="186" alt="530075472-e7d44b0a-cdaf-49dd-b07c-2b4b42058262" src="https://github.com/user-attachments/assets/366c6a7f-af36-459b-a5a4-6a61fda9e01f" />

## Result
Thus , the program has been executed succesfully.



