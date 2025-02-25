# LeetCode 8 Patterns

This document outlines the 8 common patterns for solving problems on LeetCode. Understanding and mastering these patterns will help you approach a variety of algorithmic challenges more efficiently.

---

## 1. Sliding Window
**Concept**: A subset of elements that satisfies a given condition within a linear data structure (like an array, string, or linked list).

**Typical Input**: Linear data structure (array, string, linked list)

### Example Problem:
- **Find the longest substring with `k` unique characters in a given string**.

### Explanation:
Sliding window is a technique where you maintain a window of elements and slide it across the array or string. You expand or shrink the window to satisfy or break a certain condition. This allows you to solve problems in linear time.

---

## 2. Subset
**Concept**: Explore all possible combinations of elements from a given set. The combinations can either include repetitions or not, depending on the problem.

### Example Problem:
- **46. Permutations**

### Explanation:
Start with an empty set and, at each level, explore all possible ways to add an element to the existing subset, thereby creating a new one. The approach is similar to **Breadth-First Search (BFS)** in terms of level-by-level exploration.

---

## 3. Modified Binary Search
**Concept**: Divide the search space in half repeatedly while adjusting the logic for the specific problem requirements.

### Example Problem:
- **33. Search in Rotated Sorted Array**

### Explanation:
If the array is rotated, a typical binary search is modified to check if the middle element is part of the rotated section. Depending on the position of the target and the middle element, the search space is adjusted accordingly.

**Notes**: The binary search logic can change based on whether there are duplicates or if the target element is not found.

---

## 4. Top K Elements
**Concept**: Select `k` elements from a larger subset that satisfy a specific condition.

### Example Problem:
- **Kth Largest Element in an Array**

### Explanation:
In problems involving selecting the top `k` elements, we often use heaps (either min-heap or max-heap) to efficiently retrieve the `k` largest or smallest elements from the input array.

---

## 5. Binary Tree DFS (Depth First Search)
**Concept**: Use **Depth First Search (DFS)** to visit every node in a binary tree.

### Example Problem:
- **104. Maximum Depth of Binary Tree**

### Explanation:
DFS is typically implemented using recursion. Starting from the root node, you traverse as deep as possible along each branch before backtracking. This pattern is common for problems that require processing each node in a tree or graph.

---

## 6. Topological Sort
**Concept**: Arrange elements in a specific order when they have dependencies on each other. This is typically used for **Directed Acyclic Graphs (DAGs)**.

### Example Problem:
- **207. Course Schedule**

### Explanation:
Topological sorting helps solve problems where certain tasks (or nodes) need to be performed before others. For example, in course scheduling, you may need to complete one course before starting another. This is typically done using **BFS** or **DFS**.

---

## 7. Binary Tree BFS (Breadth First Search)
**Concept**: Explore all the nodes at the same level in a binary tree before moving to the next level.

### Example Problem:
- **102. Binary Tree Level Order Traversal**

### Explanation:
BFS uses a queue to explore nodes level by level. This approach is ideal for problems where you need to process nodes in a specific order or find the shortest path.

---

## 8. Two Pointer
**Concept**: Iterate through a sorted array with two pointers to solve the problem efficiently in one pass.

### Example Problem:
- **167. Two Sum II - Input Array is Sorted**

### Explanation:
Start with two pointers: one at the beginning and one at the end of the sorted array. If the sum of the two numbers is less than the target, move the left pointer to the right. If the sum is greater, move the right pointer to the left. This approach is efficient and often used for problems that require searching for pairs or triplets in sorted arrays.

**Also used in**:
- **3Sum**: A common problem where you need to find all unique triplets in an array that sum to a specific target.
---

By following this structured approach, you'll be able to efficiently solve problems on LeetCode using these common patterns.

---

**Note**: Always make sure to read the problem carefully to identify which pattern is the most appropriate for a given problem. Understanding these patterns will help you break down complex problems into more manageable subproblems.
