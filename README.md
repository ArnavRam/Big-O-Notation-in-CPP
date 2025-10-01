# Experiment 22 - To study and implement Algorithm analysis using Big O notation

---

## Aim
- To study and understand **Big O Notation** in C++ for analyzing the **time and space complexity** of algorithms.
- To implement simple programs that demonstrate different common complexities.

---

## Tools Used
- Visual Studio Code
- MinGW-w64 with g++ Compiler

---

## Theory
**Big O Notation** is a mathematical notation used in computer science to describe the performance or complexity of an algorithm. It specifically describes the **upper bound** or worst-case scenario, focusing on how the running time or space requirements grow as the input size (`n`) approaches infinity.

### Key Characteristics
- **Asymptotic Analysis:** Focuses on the growth rate for very large inputs.
- **Machine Independent:** Ignores constants and hardware-specific details.
- **Worst-Case Scenario:** Provides a guarantee on the performance.
- **Simplification:** Ignores constants and lower-order terms (e.g., O(2n + 10) becomes O(n)).

### Common Time Complexities
- **O(1) - Constant Time:** The execution time is constant, regardless of the input size (e.g., accessing an array element by index).
- **O(log n) - Logarithmic Time:** The time increases logarithmically as the input size grows (e.g., binary search).
- **O(n) - Linear Time:** The time is directly proportional to the input size (e.g., iterating through an array).
- **O(n log n) - Linearithmic Time:** A common complexity for efficient sorting algorithms (e.g., Merge Sort, Quick Sort).
- **O(n²) - Quadratic Time:** The time is proportional to the square of the input size (e.g., nested loops, bubble sort).
- **O(2ⁿ) - Exponential Time:** The time doubles with each addition to the input dataset, becoming very slow very quickly (e.g., recursive Fibonacci calculation).

---

## Algorithm / Logic

### Program 1: Demonstrating O(1) – Constant Time
1.  **Start**
2.  Declare and initialize an array.
3.  Access and print a single element at a specific index (e.g., `arr[3]`).
4.  This operation takes the same amount of time regardless of the array's size.
5.  **End**

### Program 2: Demonstrating O(n) – Linear Time
1.  **Start**
2.  Declare an array of size `n`.
3.  Use a single `for` loop that iterates from `0` to `n-1`.
4.  Inside the loop, perform a simple operation like printing the element.
5.  The total number of operations is directly proportional to `n`.
6.  **End**

### Program 3: Demonstrating O(n²) – Quadratic Time
1.  **Start**
2.  Declare an array of size `n`.
3.  Use a nested `for` loop structure. The outer loop runs from `i=0` to `n-1`, and the inner loop runs from `j=0` to `n-1`.
4.  Inside the inner loop, print the pair of indices `(i, j)`.
5.  The total number of operations is `n * n`, or n².
6.  **End**

### Program 4: Demonstrating O(log n) – Logarithmic Time (Binary Search)
1.  **Start**
2.  Use a sorted array of size `n`.
3.  Implement the binary search algorithm, which repeatedly divides the search interval in half.
4.  The number of comparisons required to find an element grows logarithmically with the size of the array.
5.  **End**

---

## Conclusion
Big O Notation provides a standardized and essential framework for measuring and comparing the efficiency of algorithms. By focusing on the asymptotic behavior, it allows developers to predict how an algorithm will scale with larger inputs, ignoring machine-specific details. This experiment demonstrated how different code structures lead to different complexities, from the highly efficient O(1) to the inefficient O(n²). Mastering Big O analysis is crucial for writing optimized code, passing technical interviews, and making informed decisions in software engineering.
