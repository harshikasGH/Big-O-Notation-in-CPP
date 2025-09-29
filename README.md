Big O Notation in C++

Aim  
To study and understand **Big O Notation** in C++ for analyzing the **time and space complexity** of algorithms, and to implement simple programs that demonstrate different complexities.

Theory  
**Big O Notation** is a mathematical notation used to describe the **upper bound** of an algorithm’s growth rate. It provides a way to classify algorithms according to how their running time or space requirements grow as the input size increases.

### Characteristics of Big O Notation  
- **Asymptotic Analysis**: Focuses on growth rate as input size `n → ∞`.  
- **Machine Independent**: Ignores hardware and implementation details.  
- **Upper Bound**: Describes the worst-case scenario.  
- **Simplification**: Ignores constants and lower-order terms.  

### Common Time Complexities  
- **O(1)** → Constant time (independent of input size).  
- **O(log n)** → Logarithmic time (binary search).  
- **O(n)** → Linear time (linear search).  
- **O(n log n)** → Linearithmic time (merge sort, quick sort average).  
- **O(n²)** → Quadratic time (bubble sort, selection sort).  
- **O(2<sup>n</sup>)** → Exponential time (recursive Fibonacci).  
- **O(n!)** → Factorial time (brute-force permutations).  

## Algorithms Demonstrating Big O  

### O(1) – Constant Time  
1. Start  
2. Access an element in an array by index.  
3. Print the element.  
4. End  


### O(n) – Linear Time  
1. Start  
2. Input array of size `n`.  
3. For each element from `0` to `n-1`:  
   - Print element.  
4. End  


### O(n²) – Quadratic Time  
1. Start  
2. Input array of size `n`.  
3. For `i = 0` to `n-1`:  
   - For `j = 0` to `n-1`:  
     - Print pair `(i, j)`.  
4. End  

### O(log n) – Logarithmic Time (Binary Search)  
1. Start  
2. Input sorted array and key.  
3. Initialize `low = 0`, `high = n-1`.  
4. While `low <= high`:  
   - Compute `mid = (low + high)/2`.  
   - If `arr[mid] == key`, return index.  
   - Else if `arr[mid] > key`, set `high = mid - 1`.  
   - Else set `low = mid + 1`.  
5. If not found, print "Element not found".  
6. End  


### O(2<sup>n</sup>) – Exponential Time (Recursive Fibonacci)  
1. Start  
2. Define recursive function `fib(n)`:  
   - If `n <= 1`, return `n`.  
   - Else return `fib(n-1) + fib(n-2)`.  
3. Call `fib(n)` for input `n`.  
4. End  


## Time Complexity Comparison  

| Complexity | Example Algorithm        | Growth Rate |
|------------|--------------------------|-------------|
| O(1)       | Array element access     | Constant    |
| O(log n)   | Binary Search            | Slow growth |
| O(n)       | Linear Search            | Linear      |
| O(n log n) | Merge Sort, Quick Sort   | Linearithmic|
| O(n²)      | Bubble Sort, Selection   | Quadratic   |
| O(2<sup>n</sup>)     | Recursive Fibonacci      | Exponential |
| O(n!)      | Brute-force permutations | Factorial   |


## Applications  

- **Algorithm Analysis** → Compare efficiency of algorithms.  
- **Data Structures** → Evaluate operations like insertion, deletion, search.  
- **Optimization** → Choose the most efficient algorithm for large inputs.  
- **Software Engineering** → Estimate scalability and performance.  

## Conclusion  

- Big O Notation provides a **standardized way** to measure algorithm efficiency.  
- It focuses on **asymptotic behavior**, ignoring constants and lower-order terms.  
- Different algorithms with the same functionality can have drastically different complexities.  
- Mastering Big O is essential for **competitive programming, interviews, and real-world software optimization**.
