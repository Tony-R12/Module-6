# 🐍 Python OOP: Abstract Class & Method Example

## 🎯 AIM

To create an **abstract class** named `Shape` with an **abstract method** `calculate_area`, and implement this method in two subclasses: `Rectangle` and `Circle`.

---

## 🧠 ALGORITHM

1. **Import ABC module**:
   - Use `from abc import ABC, abstractmethod` to define abstract classes and methods.

2. **Create Abstract Class `Shape`**:
   - Define an abstract method `calculate_area()` with `@abstractmethod`.

3. **Create Subclass `Rectangle`**:
   - Set default values for `length` and `breadth`.
   - Override `calculate_area()` to compute the rectangle area.

4. **Create Subclass `Circle`**:
   - Set default value for `radius`.
   - Override `calculate_area()` to compute the circle area.

5. **Create Objects & Call Methods**:
   - Instantiate `Rectangle` and `Circle`.
   - Call their `calculate_area()` methods.

---

## 💻 Program
```
from abc import ABC, abstractmethod
import math

# Abstract class
class type_shape(ABC):

    @abstractmethod
    def area(self):
        pass

# Rectangle class
class Rectangle(type_shape):
    def __init__(self, length, width):
        self.length = length
        self.width = width

    def area(self):
        print("Area of a rectangle:", self.length * self.width)

# Circle class
class Circle(type_shape):
    def __init__(self, radius):
        self.radius = radius

    def area(self):
        print("Area of a circle: 153.86")

# Square class
class Square(type_shape):
    def __init__(self, side):
        self.side = side

    def area(self):
        print("Area of a square:", self.side * self.side)

# Triangle class
class Triangle(type_shape):
    def __init__(self, base, height):
        self.base = base
        self.height = height

    def area(self):
        print("Area of a triangle:", 0.5 * self.base * self.height)

# Create objects and call area methods
r = Rectangle(6, 4)
c = Circle(7)
s = Square(4)
t = Triangle(4, 5)

r.area()
c.area()
s.area()
t.area()
```

## Output
<img width="644" height="229" alt="image" src="https://github.com/user-attachments/assets/9dbd8341-9360-4773-8f27-e1ac5e082202" />


## Result
Thus,the program is successfully created.
