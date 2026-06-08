# # ➖ Matrix Operations-Matrix Subtraction in Python

## 🎯 AIM:
To write a Python program that reads two matrices from the user and performs matrix subtraction.

---

## 🧠 ALGORITHM:

1. **Start**
2. Create variables `r` and `c` for rows and columns
3. Get the values of `r` and `c` from the user
4. Define a function `create_matrix(n, m)` to:
   - Prompt user for each matrix element
   - Append each row to form a complete matrix
5. Call the `create_matrix()` function twice to read two matrices `A` and `B`
6. Define a loop to subtract the elements of matrix `B` from matrix `A`
7. Store the result in a new matrix `C`
8. Print the resulting matrix `C`
9. **Stop**

---

## 💻 PROGRAM:
```
def create_matrix(n, m):
    print(f"Enter the elements of a {n}x{m} matrix:")
    matrix = []
    for i in range(n):
        row = list(map(int, input().split()))
        matrix.append(row)
    return matrix

r = int(input("Enter number of rows: "))
c = int(input("Enter number of columns: "))

print("\nMatrix A:")
A = create_matrix(r, c)

print("\nMatrix B:")
B = create_matrix(r, c)

C = []
for i in range(r):
    row = [A[i][j] - B[i][j] for j in range(c)]
    C.append(row)

print("\nResult of Matrix A - Matrix B:")
for row in C:
    print(' '.join(map(str, row)))
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/be40dbd7-ea47-4cc3-8692-f4927e4c6082)

## RESULT:
Thus,the program is executed successfully
