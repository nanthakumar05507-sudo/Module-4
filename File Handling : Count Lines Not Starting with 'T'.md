# File Handling in Python: Count Lines Not Starting with 'T'

## 🎯 Aim
To write a Python program that counts the number of lines in a text file `story.txt` that do **not** start with the alphabet `'T'`.

## 🧠 Algorithm
1. Open the file `story.txt` in **read mode**.
2. Initialize a counter `count` to zero.
3. Iterate through each line of the file:
   - Check if the first character of the line is **not** `'T'`.
   - If the line does not start with `'T'`, increment the `count` by 1.
4. After processing all lines, print the `count` value, which represents the number of lines that do not start with `'T'`.

## 🧾 Program
```
from collections import defaultdict


def create_file(file_path, content):
    with open(file_path, 'w') as file:
        file.write(content)

# Function to calculate character frequencies
def char_frequency(file_path):
    freq = defaultdict(int)
    with open(file_path,'r') as file:
        for line in file:
            for char in line:
                freq[char]+=1
    return freq
```
## Output
<img width="1226" height="298" alt="image" src="https://github.com/user-attachments/assets/d0a3fb3c-c810-4bd3-a5f2-14f3d8451a05" />

## Result
Thus the output is Verified.
