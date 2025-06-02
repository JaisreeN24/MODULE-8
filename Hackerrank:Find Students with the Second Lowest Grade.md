# 🎓 Hackerrank:Python Program to Find Students with the Second Lowest Grade

This program reads student names and their corresponding grades, identifies the **second lowest grade**, and prints the names of all students who have that grade in **alphabetical order**.

---

## 🎯 Aim

To write a Python program to:
- Read a list of students and their grades.
- Identify the second lowest grade.
- Print the names of students who have that grade, sorted alphabetically.

---

## 🧠 Algorithm

1. **Read** an integer `n` representing the number of students.
2. **Read** each student’s name and grade, and store them as a sublist inside a list.
3. **Extract** all the grades and sort them.
4. **Identify** the second lowest grade from the sorted grade list.
5. **Collect** names of all students whose grade matches the second lowest grade.
6. **Sort** the names alphabetically.
7. **Print** each name on a new line.

---

## 💻  Program

    n = int(input())
    students = []
    for _ in range(n):
        name = input()
        grade = float(input())
        students.append([name, grade])
    
    grades = sorted({s[1] for s in students})
    second_lowest = grades[1] if len(grades) > 1 else grades[0]
    
    result = sorted([s[0] for s in students if s[1] == second_lowest])
    print('\n'.join(result))
## Output
![image](https://github.com/user-attachments/assets/a1d8e5c1-e78e-4120-9bfa-0fd2350f5590)

## Result
Thus, the program to Read a list of students and their grades, Identify the second lowest grade, Print the names of students who have that grade, sorted alphabetically is executed and verified successfully.

