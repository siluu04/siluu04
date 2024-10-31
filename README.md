# Assingnment-1









# Assingnment-2
Advanced Array and String Operations with Complexity Analysis


# Multi-dimensional Array Operations

Implementing a TwoDimensionalArray class with methods to handle row-wise and column-wise insertion, deletion, traversal.

![image](https://github.com/user-attachments/assets/fc28d3b4-9f0a-4080-ac12-928d714980a7)

# Matrix transposition with class MatrixOperations

![image](https://github.com/user-attachments/assets/3035fe35-e509-494a-8cdd-5bd8c5d1589d)

# Test cases

![image](https://github.com/user-attachments/assets/6d5a621a-5d77-4a41-8660-e07a88f4fa84)





# Advanced String Operations:
 Implementing StringAlgorithms class for pattern matching using KMP and string compression using RLE.

# Steps

# KMP Pattern Matching:

Implement the Knuth-Morris-Pratt (KMP) algorithm for substring search. Create an indexOfKMP method to return the starting index of a pattern in the text.

# Run Length Encoding (RLE):

Write the runLengthEncoding method to perform RLE on an input string, compressing sequences of identical characters.

![image](https://github.com/user-attachments/assets/b9d625ca-1af2-4a72-968e-cbd40d8ed5ad)

![image](https://github.com/user-attachments/assets/f84ff7c4-96ae-408c-8d7b-49b963d88860)

# Test cases

![image](https://github.com/user-attachments/assets/1b9b9fa8-56b3-4948-b3ce-3f4eedd3453c)





# Complexity Analysis

# 1. KMP Pattern Matching Algorithm

 # Time Complexity:
- Best Case: Ω(n) 
  - The pattern matches with the text without any mismatches, where n is the length of the text.
  
- Average Case: Θ(n + m)
  - The average case occurs when characters are matched and mismatches are few. Here, m is the length of the pattern.

- Worst Case: O(n + m)
  - In the worst case, every character of the text is compared with the characters of the pattern, resulting in linear complexity.

# Space Complexity:
- The space complexity is O(m) for the LPS array, where m is the length of the pattern. The algorithm uses a fixed amount of space for the LPS array regardless of the text size.

# 2. Run Length Encoding (RLE)

# Time Complexity:
- Best Case: Ω(n)
  - The best case occurs when all characters are different. The algorithm still needs to iterate through the entire input string of length n.

- Average Case: Θ(n)
  - On average, the algorithm processes each character, leading to linear time complexity.

- Worst Case: O(n)
  - In the worst case, all characters are the same (e.g., "aaaaaa"), the algorithm still examines all characters, resulting in linear time complexity.

# Space Complexity:
- The space complexity is O(n) in the worst case, where the output size can be the same as the input size. For example, the string "abc" would result in "1a1b1c", which maintains linear space.

Summary:

- KMP Pattern Matching:
  - Time Complexity: Best: Ω(n), Average: Θ(n + m), Worst: O(n + m)
  - Space Complexity: O(m)

- Run Length Encoding:
  - Time Complexity: Best: Ω(n), Average: Θ(n), Worst: O(n)
  - Space Complexity: O(n)







