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
```python
class Generate:

def __init__(self, first,d,last):

    self.first = first
    
    self.d = d
    
    self.last=last

def Ap_generate(self):

    L=[i for i in range(self.first,self.last+1,self.d)]
    
    return L
Series = Generate(200,2,301)

print(Series.Ap_generate())
```
## OUTPUT:
<img width="1259" height="173" alt="491490639-7c527f99-e2ed-4980-b9ba-be7904bae4f4" src="https://github.com/user-attachments/assets/1d2b3df9-08d6-4f93-b7a7-8ad7a82f8801" />


## RESULT:
the program is excuted and verified.

## 🧮 List Comprehension:Scalar multiple of a set of numbers
## 🎯 AIM:
To write a Python program to store a scalar multiple of a set of numbers in a list using list comprehension.

## 🧠 ALGORITHM:
1. Read n (number of elements).
2. Read scl (scale factor).
3. Initialize empty list l. For i = 1 to n:
4. Read a float x, append to l.
5. Compute sq_l = [item * scl for item in l].
6. Print l and sq_l.
   
## 💻 PROGRAM:
```python
n=int(input())

scl=int(input())

l=[]

for i in range(n):

x=float(input())

l.append(x)
sq_l=[item*scl for item in l]

print(l)

print(sq_l)
```
OUTPUT:
<img width="941" height="429" alt="491492870-43ef61ae-5673-42e5-aa90-80cbca9f7184" src="https://github.com/user-attachments/assets/88afa6c8-8f93-4d87-8ecb-692c6fc25438" />


RESULT:
Thus, the program has been executed and verified successfully.

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
```python
rows=int(input())

columns=int(input())

matrix=[[0]*columns for row in range(rows)]

for i in range(rows):

lines=list(map(int, input().split()))

for j in range(columns):

    matrix[i][j]=lines[j]
print(matrix)

for i in range(rows):

for j in range(columns):

    if(i==j):
    
        print(matrix[i][j],end=" ")
   
    else:
    
        print(' ',end=" ")

print()
```
### Output:

<img width="961" height="399" alt="491491379-d6e313de-9e74-4482-84b4-264b975b54ef" src="https://github.com/user-attachments/assets/00f675e8-531b-4bad-bcb1-3af7f88ce425" />

## Result
The program is excuted and verified

## ➖ Matrix Operations-display the lower triangle matrix
## 🎯 AIM:
To write a Python program to read a matrix and display the lower triangle Matrix.

## 🧠 ALGORITHM:
1. Input n (size of square matrix).
2. Initialize an n × n matrix.
3. For each row, read n integers and store them in the matrix.
4. Print "Matrix:".
5. For each element M[i][j]: If i ≥ j, print M[i][j]. Else, print 0.
6. Move to a new line after each row.
   
## 💻 PROGRAM:
```python
def read_matrix(n):

matrix=[[0]*n for row in range(n)]

for i in range(n):

    lines=list(map(int,input().split()))
    
    for j in range(n):
    
        matrix[i][j]=lines[j]

return matrix
def print_matrix(M):

print("Matrix:")

for i in range(len(M)):

    for j in range(len(M[0])):
    
        if(i>j or i==j):
        
            print(M[i][j],end=" ")
       
        else:
        
            print(0,end=" ")
   
    print()
```
    
## OUTPUT:
<img width="665" height="413" alt="491494455-7baf92c7-068c-4c0b-b183-fc5b3aeedfb4" src="https://github.com/user-attachments/assets/a304cd5a-ae00-4d0a-bf16-e1e1e9cb9161" />


RESULT:
Thus, the program has been executed and verified successfully.

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
