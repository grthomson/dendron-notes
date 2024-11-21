---
id: el4vn10duywyad1juduzr54
title: big-O-notation
desc: ''
updated: 1732215255112
created: 1732215122026
---

# Big O Notation

Big O notation describes the **efficiency** of an algorithm in terms of:
1. **Time Complexity**: How runtime grows as input size (`n`) increases.
2. **Space Complexity**: How memory usage grows with input size.

## Key Concepts
- Focuses on the **worst-case scenario**.
- **Ignore constants** and low-order terms (e.g., \(2n + 5\) simplifies to \(O(n)\)).
- Common complexities (from fastest to slowest):
  - \(O(1)\): Constant time (e.g., accessing an array element).
  - \(O(\log n)\): Logarithmic (e.g., Binary Search).
  - \(O(n)\): Linear (e.g., iterating through an array).
  - \(O(n \log n)\): Linearithmic (e.g., Merge Sort).
  - \(O(n^2)\): Quadratic (e.g., Bubble Sort).

## Worked Example: Sorting
### Problem
Sort an array of \(n\) numbers using Merge Sort.

### Steps
1. **Divide** the array into two halves (\(\log n\) levels of division).
2. **Merge** sorted halves back together (\(O(n)\) work per level).

### Total Time Complexity
\[
O(n \cdot \log n)
\]

### Why Logarithms?
- Dividing into halves involves \(\log_2 n\) levels (base-2 logarithms).
- At each level, \(n\) elements are processed.

### Example Calculation
For \(n = 8\), Merge Sort:
- Divides: \(8 \to 4 \to 2 \to 1\) (\(3 = \log_2(8)\)).
- Merges: Each level processes all 8 elements.
- Total Work: \(O(8 \cdot \log_2 8) = O(24)\).

## Notes
- Base of \(\log n\) is usually implied as 2 in computational contexts.
- Big O ignores constants, so \(O(2n)\) simplifies to \(O(n)\).