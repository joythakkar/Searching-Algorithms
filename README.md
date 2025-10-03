# Searching-in-CPP


## Aim
To study and implement searching algorithms in C++.

---

## Theory

### What are Algorithms?
An **algorithm** is a step-by-step set of instructions designed to solve a problem or perform a task, converting input data into a desired output.

---

### Searching
Searching algorithms are essential tools in computer science used to locate specific items within a collection of data.  
When we search for an item in an array, the two most common algorithms are:

####  Linear Search
- Used for **unsorted arrays**.  
- Compares each element one by one with the target.  
- Time Complexity: **O(n)**.  

#### 🔹 Binary Search
- Used for **sorted arrays**.  
- Compares the middle element first.  
- If the middle element matches the target, it is returned.  
- Otherwise, the search continues in the left or right half depending on the comparison.  
- Time Complexity: **O(log n)**.  

---

## Algorithms

### Linear Search
1. A vector/array `arr` of size `n`.  
2. A target value to search.  
3. Return `1` if the element is found, otherwise `-1`.  
4. Set `i = 0`.  
5. Repeat while `i < n`:  
   - If `arr[i] == target`, return `1`.  
   - Else, increment `i = i + 1`.  

---

### Binary Search
1. A **sorted** vector/array `arr` of size `n`.  
2. A target value to search.  
3. Return the index of the element if found, otherwise `-1`.  
4. Start with: `low = 0`, `high = n - 1`.  
5. Repeat while `low <= high`:  
   - Compute `mid = low + (high - low) / 2`.  
   - If `arr[mid] == target`, return `mid`.  
   - If `arr[mid] < target`, update `low = mid + 1`.  
   - Else, update `high = mid - 1`.  
6. If the loop ends without finding the target, return `-1`.  

---

## Conclusion
We learnt about **algorithms** and two main types of searching algorithms:  
- **Linear Search** → best for unsorted arrays.  
- **Binary Search** → efficient for sorted arrays.  
