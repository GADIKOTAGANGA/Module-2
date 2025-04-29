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
def is_palindrome(num):
    num_str = str(num)
    return num_str == num_str[::-1]
number=int(input()) 
if is_palindrome(number):
    print(f"The given number {number} is a Palindrome")
else:
    print(f"The given number {number} is not a palindrome")
```
## Output
![Screenshot 2025-04-29 180939](https://github.com/user-attachments/assets/2f5f668b-ec5d-4839-91aa-0b83be5988a9)

## Result
The expected output is excuted
