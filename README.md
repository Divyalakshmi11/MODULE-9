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

# 🧮 List Comprehension:Transpose of Matrix 

## 🎯 AIM:
To write a Python program to compute the **transpose** of a matrix using **list comprehension**.

---

## 🧠 ALGORITHM:

1. **Start**
2. Create variables `r` and `c` to represent the number of rows and columns of the matrix.
3. Get the values of `r` and `c` from the user.
4. Define a function `create(r, c)` to create the matrix by reading the elements from the user.
5. Use **list comprehension** to calculate the transpose of the matrix.
6. Print the transposed matrix.
7. **Stop**

---

## 💻 PROGRAM:
```
def create(r, c):
    matrix = []
    for i in range(r):
        row = list(map(int, input().split()))
        matrix.append(row)
    return matrix

r = int(input())
c = int(input())

matrix = create(r, c)

transpose = [[matrix[j][i] for j in range(r)] for i in range(c)]

for row in transpose:
    print(*row)
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/ca26d82a-9f6e-40b9-b002-cc4741ef8968)


## RESULT:
The program successfully transposes a matrix using list comprehension and prints the result as expected.

# Matrix Operations-Diagonal Matrix Elements Printer 🧮

This Python program reads a matrix of any size from the user and prints **only the diagonal elements**, leaving other elements blank in the output.

## 📌 Aim

To write a Python program that prints only the diagonal elements of a given matrix.

## 🧠 Algorithm

1. Read the number of rows and columns from the user.
2. Initialize an empty matrix of size `rows × columns`.
3. Populate the matrix with user input.
4. Display the full matrix.
5. Iterate through the matrix and:
   - If `i == j`, print the element (main diagonal).
   - Else, print a blank space.
6. Print a newline after each row.

## 🖥️ Program
```
rows = int(input("Enter number of rows: "))
cols = int(input("Enter number of columns: "))

print("Enter the elements row by row:")
matrix = []
for i in range(rows):
    row = list(map(int, input().split()))
    matrix.append(row)

print("\nFull matrix:")
for row in matrix:
    print(' '.join(map(str, row)))

print("\nDiagonal elements:")
for i in range(rows):
    for j in range(cols):
        if i == j:
            print(matrix[i][j], end=' ')
        else:
            print(' ', end=' ')
    print()
```

### Output:
![image](https://github.com/user-attachments/assets/fe77b35f-8ed7-49a5-b018-cbb80bb2b697)

## Result
Thus,the program is executed successfully
