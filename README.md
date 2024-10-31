# Assingnment-1

Implementing and Analyzing Basic Data Structures


# Static array has a fixed size, and lets perform operations such as insertion, deletion, and traversal on it.

#staticarray.java implementation
![image](https://github.com/user-attachments/assets/a355b365-34d0-45f4-aa76-5b3a4a16b941)


# Dynamic arrays expand their capacity, allowing flexibility and variablity in size.

#dynamicarray.java implementation
![image](https://github.com/user-attachments/assets/a33ae373-d260-4b41-91ee-616b959656b9)


# Algorithm Analysis

#Analysis of the time complexity for each implemented method.

# Static Array
•	Insertion: O(1) if there’s space available.

•	Deletion: O(n) since all elements need shifting after deletion.

•	Traversal: O(n) as every element is visited.

# Dynamic Array
•	Insertion: O(1) due to resizing only when needed.

•	Deletion: O(n) because of shifting elements.

•	Traversal: O(n)

# Test cases

# Static array test cases:

![image](https://github.com/user-attachments/assets/d9a20f97-df8f-4395-b412-08c564ee3e8f) 


# Dynamic array test cases:

![image](https://github.com/user-attachments/assets/c4e8d71b-6f9c-437e-bf5d-30df76bf7174)


# String Operations:

#The stringoperations class includes methods for concatenation, substring extraction, comparison, and frequency counting.

stringoperation.java implementation

![image](https://github.com/user-attachments/assets/3b1e1275-c49b-4b85-a68d-d8714de50689) 


![image](https://github.com/user-attachments/assets/30fd41e6-5a3d-4963-baf2-9fdabd1f51be) 




# Algorithm Analysis

# Static Array

#Static Array Operations

1.	Insertion
	Time Complexity: O(1) (if inserting at the end) or O(n) (if inserting at a specific index that requires shifting elements).
	Space Complexity: O(n), where n is the size of the array.

2.	Deletion
	Time Complexity: O(1) (if deleting the last element) or O(n) (if deleting from an index that requires shifting elements).
	Space Complexity: O(n)).

3.	Traversal
	Time Complexity: O(n)), where n is the number of elements.
	Space Complexity: O(1) since it requires no additional space.


# Dynamic Array

#Dynamic Array Operations

1.	Insertion
	Time Complexity: O(1)for most insertions. However, during resizing (when capacity is reached), it takes O(n) time to copy elements to a new array.
	Space Complexity: O(n), where n is the number of elements in the array.

2.	Deletion
	Time Complexity: O(1)(last element) or O(n) (with shifting).
	Space Complexity: O(n)

3.	Traversal
	Time Complexity: O(n)
	Space Complexity: O(1)


# String Operations

1.	Concatenation
	 Time Complexity: O(m+n), where m and n are the lengths of the two strings.
	 Space Complexity: O(m+n) for creating a new concatenated string.

2.	Substring
	Time Complexity: O(k), where k is the length of the substring.
	Space Complexity: O(k)) for storing the substring.

3.	Comparison
	Time Complexity: O(min⁡(m,n)), where m and n are the lengths of the two strings.
	Space Complexity: O(1) since no additional space is needed.

4.	Character Frequency
	Time Complexity: O(n), where n is the length of the string.
	Space Complexity: O(n) for storing frequencies of each character.


# 1. Binary Search
   It is used to find the position of an element in a sorted array. Each time, it halves the search space, leading to a recurrence relation that describes this behavior.

The recurrence relation for binary search can be expressed as:

•	T(n)=T(n/2)+O(1)T(n) 

 where,
•	T(n)): The time complexity of binary search for an input of size nnn.
•	T(n/2) Recursive call on half the array size.
•	O(1) Constant time work done per step (e.g., comparing the middle element).


Solution by Recurrence Tree:

1.	Unrolling the recurrence:
	T(n)=T(n/2)+O(1)
	T(n)=T(n/4)+O(1)+O(1)
	T(n)=T(n/8)+O(1)+O(1)+O(1)
	Continuing this way leads to T(n)=T(n/2k)+k⋅O(1)

2.	Base case:
•	We reach T(1) when n/2k=1

3.	Final Solution:
•	Substituting k=log⁡2(n),we find T(n)=O(log⁡n)

#      Result:
•	Time Complexity: O(log⁡n)

•	Space Complexity: O(log⁡n) due to the recursion stack.



# 2. Merge Sort
   Merge sort divides the array into two halves and then merges them.
   

The recurrence relation for merge sort is:

•	T(n)=2⋅T(n/2)+O(n)

where,
•	2⋅T(n/2)2): Two recursive calls on each half of the array.
•	T(n)): Time complexity for merge sort on input of size nnn.
•	O(n)): Time to merge two halves (linear).


Solution using Master Theorem: The recurrence relation fits the form:

•	T(n)=a⋅T(n/b)+f(n)
•	Here, a=2a, b=2b, and f(n)=O(n)

To apply the Master Theorem, calculate nlog⁡b(a)n^{\log_b(a)}nlogb(a):

•	Since log⁡2(2)=1nlog2(2)=O(n)
•	Since f(n)=O(n), we match Case 2 of the Master Theorem, where f(n)=O(nlog⁡b(a))

# Result:
•	Time Complexity: O(n log⁡n)

•	Space Complexity: O(n), as merging requires temporary space.











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







