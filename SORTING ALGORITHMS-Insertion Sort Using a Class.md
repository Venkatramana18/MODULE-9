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
```python
class Numbers: def init(self): self.lst = []

def create_list(self):
    n = int(input())
    self.lst = [int(input()) for _ in range(n)]

def sorting(self):
    n = len(self.lst)
    for i in range(n):
        for j in range(0, n - i - 1):
            if self.lst[j] > self.lst[j + 1]:
                self.lst[j], self.lst[j + 1] = self.lst[j + 1], self.lst[j]

def print_List(self):
    for num in self.lst:
        print(num) 
```
        

## OUTPUT:

<img width="874" height="649" alt="491491972-7c379537-aed7-4649-ae96-b2fa60471a9d" src="https://github.com/user-attachments/assets/00d3192e-9b70-4fbd-9c3a-ecb7a0b56952" />

## RESULT:
The program is excuted and verified.
ADD CODE HERE
