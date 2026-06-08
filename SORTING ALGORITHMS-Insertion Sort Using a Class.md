# 🧮 SORTING ALGORITHMS: Insertion Sort Using a Class

This program demonstrates how to implement the **Insertion Sort algorithm** using a Python class. It allows the user to input a list of numbers, sorts them using the insertion sort technique, and displays the sorted list.

---

## 🎯 Aim

To develop a Python class with functions to:
- Create a list of integers
- Sort it using the **Insertion Sort** algorithm
- Display the sorted list

---

## 🧠 Algorithm

1. **Start the program**
2. **Define a class** `InsertionSorter`
3. Inside the class:
   - `create_list()`:
     - Read number of elements
     - Store them in a list
   - `insertion_sort()`:
     - Iterate from the second element to the end
     - Move elements greater than the key to one position ahead
     - Insert the key at the correct position
   - `print_list()`:
     - Print the sorted list
4. **Create an object** of the class
5. **Call** the methods in order: `create_list()`, `insertion_sort()`, and `print_list()`
6. **End the program**

---

## 💻 PROGRAM:
```
class InsertionSorter:
    def __init__(self):
        self.data = []

    def create_list(self):
        n = int(input("Enter number of elements: "))
        self.data = list(map(int, input(f"Enter {n} integers: ").split()))

    def insertion_sort(self):
        for i in range(1, len(self.data)):
            key = self.data[i]
            j = i - 1
            while j >= 0 and self.data[j] > key:
                self.data[j + 1] = self.data[j]
                j -= 1
            self.data[j + 1] = key

    def print_list(self):
        print("Sorted list:", self.data)

# Create an object of InsertionSorter class
sorter = InsertionSorter()

# Call methods in order
sorter.create_list()
sorter.insertion_sort()
sorter.print_list()
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/c7c93059-47b5-4444-be67-d0b15dbb8fa4)

## RESULT:
Thus,the program is executed successfully
