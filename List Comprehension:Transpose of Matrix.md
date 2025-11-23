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


