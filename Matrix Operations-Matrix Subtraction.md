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


## RESULT:
Thus, the program has been executed and verified successfully.
