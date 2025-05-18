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
```
rows = int(input())
cols = int(input())

matrix = []
for i in range(rows):
    row = list(map(int, input().split()))
    matrix.append(row)

for row in matrix:
    print(*row)

print("Main diagonal elements:")
for i in range(rows):
    for j in range(cols):
        if i == j:
            print(matrix[i][j], end=" ")
        else:
            print(" ", end=" ")
    print()
```

### Output:
![image](https://github.com/user-attachments/assets/9668e1c6-ff6f-4c2d-870a-11d69a0976c4)


## Result
The program successfully displays the input matrix and prints only the main diagonal elements by checking the condition i == j. Blank spaces are used for non-diagonal positions to maintain the matrix structure visually.
