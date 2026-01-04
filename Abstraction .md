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

class type_shape(ABC):
    @abstractmethod
    def area(self):
        pass

class Rectangle(type_shape):
    def __init__(self, length, width):
        self.length = length
        self.width = width
    
    def area(self):
        return self.length * self.width

class Circle(type_shape):
    def __init__(self, radius):
        self.radius = radius
    
    def area(self):
        return round(3.14 * self.radius * self.radius, 2)


rect = Rectangle(3, 5)
circle = Circle(4)

print("Area of a rectangle:", rect.area())
print("Area of a circle:", circle.area())
```

## Output
<img width="581" height="185" alt="image" src="https://github.com/user-attachments/assets/5f5d2df7-dc5f-479f-9e07-0adf408ee82f" />



## Result
Thus, the program has been successfully executed.
