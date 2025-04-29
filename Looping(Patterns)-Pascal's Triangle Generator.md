# 🔺 Looping(Patterns)-Pascal's Triangle Generator in Python

This project demonstrates a simple Python program to generate **Pascal’s Triangle**, where the number of rows is provided by the user.

---

## 🎯 Aim

To write a Python program that generates **Pascal's Triangle** using numbers. The number of rows is accepted from the user.

---

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

---

## 🧪 Program
```
def pascel_triangle(n):
    triangle=[]
    for i in range(n):
        row=[1]
        if triangle:
            last_row=triangle[-1]
            for j in range (len(last_row)-1):
                row.append(last_row[j]+last_row[j+1])
            row.append(1)
        triangle.append(row)
    for row in triangle:
        print(" ".join(map(str , row)))
num_rows=int(input())
pascel_triangle(num_rows)
```

## Sample Output
![Screenshot 2025-04-29 175752](https://github.com/user-attachments/assets/6bdcdb38-1f03-46a1-a9b8-f12b25b0593e)

## Result
The expected output is acheived
