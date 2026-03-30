# 📐 Taylor Series:sinh(x) Evaluation using Recursion in Python

## 🎯 AIM:
To write a Python program to evaluate the value of **sinh(x)** for **n terms** using recursion.

---

## 🧠 ALGORITHM:

1. **Start**
2. Read input for variable `x` (angle or number)
3. Read input for variable `n` (number of terms)
4. Define a function `fact(n)`:
   - If `n <= 1`, return 1
   - Else, return `n * fact(n - 1)` (recursive factorial)
5. Define a function `sinh(x, n)`:
   - If `n == 0`, return `x`
   - Else, return `(pow(x, 2*n + 1) / fact(2*n + 1)) + sinh(x, n - 1)`
6. Call the `sinh(x, n)` function and print the result
7. **Stop**

---

## 💻 PROGRAM:
def series(x,n):
    if n==0:
        return x
    return x**(2*n+1)/fact(2*n+1)+series(x,n-1)
def fact(n):
    if n==0:
        return 1
    return n*fact(n-1)
x=int(input())
n=int(input())
result=series(x,n)
print(result)

## OUTPUT
<img width="1137" height="269" alt="image" src="https://github.com/user-attachments/assets/9c6992cb-8561-4401-ae59-929a561712f5" />

## RESULT
Thus, the program has been execueted successfully.
