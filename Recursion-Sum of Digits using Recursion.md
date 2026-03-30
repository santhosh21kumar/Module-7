# # 🔁 Recursion:Sum of Digits using Recursion in Python

## 🎯 AIM:
To write a Python program to calculate the **sum of all digits** in a number using **recursion**.

## 🧠 ALGORITHM:

1. **Start**
2. Define a recursive function `sum_digit(n)` that:
   - Returns 0 if `n <= 0` (Base Case)
   - Else, returns `n % 10 + sum_digit(n // 10)` (Recursive Case)
3. Take integer input from the user.
4. Call the recursive function and store the result.
5. Print the result.
6. **Stop**

## 💻 PROGRAM:
l=[]
def SUM(n):
   if n==0:
      return 1
dig=n%10
l.append(dig)
SUM(n//10)
n=int(input())
SUM(n) print(sum(l))


## OUTPUT
<img width="1172" height="212" alt="image" src="https://github.com/user-attachments/assets/26b840ff-41c4-4f26-95af-a9ab7a91498d" />

## RESULT
Thus, the program has been execueted successfully.
