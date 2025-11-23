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
