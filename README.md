# 🧾 List Comprehension:Generates all even numbers between 200 and 300
## 🎯 AIM:
To write a Python class-based program that generates all even numbers between 200 and 300 using **list comprehension**, and stores them in a list.

---

## 🧠 ALGORITHM:

1. **Start**
2. Create a class named `program`
3. Create variables `a`, `b`, and `c` to represent:
   - `a`: Lower limit
   - `b`: Step value
   - `c`: Upper limit
4. Initialize the values using a constructor `__init__`
5. Define a method `display()` that uses **list comprehension** to store even numbers
6. Print the resulting list of even numbers
7. **Stop**

---

## 💻 PROGRAM:
```
class program:
    def __init__(self, a, b, c):
        self.a = a  
        self.b = b  
        self.c = c  

    def display(self):
        even_numbers = [i for i in range(self.a, self.c + 1, self.b) if i % 2 == 0]
        print("Even numbers in the given range:", even_numbers)

a = int(input("Enter the lower limit: "))
b = int(input("Enter the step value: "))
c = int(input("Enter the upper limit: "))

obj = program(a, b, c)
obj.display()
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/646b5759-11b6-49b8-bd8d-84af16e765e7)


## RESULT:
The program successfully demonstrates the use of classes, constructors, and list comprehension to display even numbers from a range with a step value.
