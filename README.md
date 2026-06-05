# Built-in Functions -Binary Conversion Using Built-in Functions in Python

## 🎯 Aim
To write a Python program to convert the number **16** into its **binary representation** using built-in Python functions.

## 🧠 Algorithm
1. Assign the value `16` to a variable `a`.
2. Use the built-in `bin()` function to convert the number to binary.
3. Print the result.

## 🧾 Program
```
a = 16
print(bin(a))
```
## Output
<img width="462" height="177" alt="Screenshot 2026-06-05 200411" src="https://github.com/user-attachments/assets/2636086e-a343-4a73-8289-ae82d115ad2b" />

## Result
Thus, the program has been excecuted successfully.


# Functions in Python: Modulo Calculator

## 🎯 Aim
To write a Python program that defines a function which accepts two values and returns their **modulo** using the `%` operator.

## 🧠 Algorithm
1. Define a function called `result` that takes two arguments `a` and `b`.
2. Inside the function, compute the modulo using `a % b`.
3. Print the result of the modulo operation.
4. Get two integer inputs from the user.
5. Call the `result` function with the user-provided values.

## 🧾 Program
```
def result(a, b):
    print(a % b)

a = int(input("Enter first number: "))
b = int(input("Enter second number: "))

result(a, b)
```
## Output
<img width="487" height="242" alt="Screenshot 2026-06-05 200514" src="https://github.com/user-attachments/assets/d75318fd-475c-4cd3-a959-aed5652574ab" />

## Result
Thus, the program has been excecuted successfully.


# Lambda Function in Python: Addition of Two Numbers

## 🎯 Aim
To write a Python program that defines a **lambda function** which takes two arguments `a` and `b`, and returns their sum.

## 🧠 Algorithm
1. Get two integer inputs from the user.
2. Use a **lambda function** to define a function `f` that returns `a + b`.
3. Call the function with the user inputs and print the result.

## 🧾 Program
```
a = int(input("Enter first number: "))
b = int(input("Enter second number: "))

f = lambda a, b: a + b
print(f(a, b))

```
## Output
<img width="497" height="228" alt="Screenshot 2026-06-05 200621" src="https://github.com/user-attachments/assets/5f7c7066-9d80-4597-9ee3-f96472a0a953" />

## Result
Thus, the program has been excecuted successfully.


# 🔺 Looping(Patterns)-Pascal's Triangle Generator in Python

This project demonstrates a simple Python program to generate **Pascal’s Triangle**, where the number of rows is provided by the user.

## 🎯 Aim

To write a Python program that generates **Pascal's Triangle** using numbers. The number of rows is accepted from the user.

## 🧠 Algorithm

1. Start the program.
2. Input the number of rows from the user.
3. Loop from 0 to the number of rows.
4. For each row:
   - Print appropriate spaces to shape the triangle.
   - Compute values using the formula:  
     \[
     C(n, k) = \frac{n!}{k!(n-k)!}
     \]
5. Print all rows of Pascal’s Triangle.
6. End the program.

## 🧪 Program
```
from math import factorial

n = int(input("Enter the number of rows: "))

for i in range(n):
    print(' ' * (n - i - 1), end='')
    for j in range(i + 1):
        print(factorial(i) // (factorial(j) * factorial(i - j)), end=' ')
    print()

```
## Sample Output
<img width="542" height="283" alt="Screenshot 2026-06-05 200730" src="https://github.com/user-attachments/assets/7b3b23c4-45d3-4c1b-af2d-db6eda13d899" />

## Result
Thus, the program has been excecuted successfully.


## Loops in Python: Palindrome Number Checker

## 🎯 Aim
To write a Python program that checks whether a given number is a **palindrome** using loops.

## 🧠 Algorithm
1. Get input from the user and assign it to a variable `num`.
2. Assign the value of `num` to a temporary variable `temp`.
3. Initialize a variable `rev` to 0 (used to store the reversed number).
4. Use a `while` loop to reverse the digits:
   - While `temp > 0`:
     - `rev = (10 * rev) + temp % 10`
     - `temp = temp // 10`
5. After the loop, compare `rev` with `num`:
   - If equal, print that the number is a palindrome.
   - Else, print that it is not a palindrome.

## 🧾 Program
```
num = int(input("Enter a number: "))
temp = num
rev = 0

while temp > 0:
    rev = (10 * rev) + temp % 10
    temp = temp // 10

if rev == num:
    print(num, "is a palindrome")
else:
    print(num, "is not a palindrome")
```
## Output
<img width="532" height="205" alt="Screenshot 2026-06-05 200854" src="https://github.com/user-attachments/assets/74d511c8-acf5-460a-8deb-bdf9b52a8bf2" />

## Result
Thus, the program has been excecuted successfully.
