# 🔄 Hackerrank : # 📦 Python Word Wrap Function

This Python program defines a function that **wraps a long string into multiple lines**, ensuring each line does not exceed a specified width.

---

## 🎯 Aim

To write a Python function that takes a long string and a specified width, and returns the string formatted with line breaks such that each line has **at most the given width**.

---

## 🧠 Algorithm

1. **Start** the program.
2. Define a function `wrap(string, max_width)`:
   - Create an empty list `wrapped_lines` to store parts of the string.
   - Loop through the string using steps of `max_width`.
   - In each iteration, extract a substring of length `max_width`.
   - Append this substring to the list.
3. Join the list with `\n` to create the final string.
4. Return the result.
5. **End** the program.

---


## 🧪 Program
      def wrap(string, max_width):
          return '\n'.join([string[i:i+max_width] for i in range(0, len(string), max_width)])
      
      # Example usage
      long_string = "This is a very long string that needs to be wrapped to fit within a specified width."
      width = 20
      wrapped = wrap(long_string, width)
      print(wrapped)
## Sample Output
![image](https://github.com/user-attachments/assets/977535bf-b74b-4382-9982-5f17f66e727a)

## Result
Thus, the program that that takes a long string and a specified width, and returns the string formatted with line breaks such that each line has **at most the given width** is executed and verfied successfully.
