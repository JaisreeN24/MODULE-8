# # 🔢 Hackerrank:# 🏆 Student Topper Finder

This Python program helps determine the **top-performing student** based on the total marks across five subjects. It uses a dictionary to store each student’s marks and identifies the topper using simple calculations and built-in functions.

---

## 🎯 Aim

To maintain a dictionary of students with their marks in five subjects, calculate their **total marks**, store them in a new dictionary, and identify the **student with the highest total (topper)**.

---

## 🧠 Algorithm

1. **Start** the program.
2. Create a dictionary `student_marks`:
   - Keys → Student names.
   - Values → List of marks in five subjects.
3. Initialize an empty dictionary `total_marks`.
4. Loop through `student_marks`:
   - Calculate the total marks using `sum()`.
   - Store the result in `total_marks`.
5. Use `max()` on `total_marks` to find the student with the highest total.
6. Print:
   - The `total_marks` dictionary.
   - The **topper's name and score**.

---

## 💻 PROGRAM:
      student_marks = {
          "Alice": [85, 90, 78, 92, 88],
          "Bob": [76, 82, 91, 87, 80],
          "Charlie": [90, 95, 89, 93, 91],
          "Diana": [81, 79, 84, 88, 85]
      }
      
      total_marks = {}
      
      for name, marks in student_marks.items():
          total_marks[name] = sum(marks)
      
      topper = max(total_marks.items(), key=lambda x: x[1])
      
      print("Total Marks:")
      for name, total in total_marks.items():
          print(f"{name}: {total}")
      
      print(f"\nTopper: {topper[0]} with {topper[1]} marks")

## OUTPUT
![image](https://github.com/user-attachments/assets/cd123a34-a7f1-4439-b0bc-7648bf8f5d18)

## RESULT
Thus the program to maintain a dictionary of students with their marks in five subjects, calculate their **total marks**, store them in a new dictionary, and identify the **student with the highest total (topper)** is executed and verified successfully.
