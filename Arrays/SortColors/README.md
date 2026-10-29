🎨 Sort Colors

A classic array problem that explores counting, in-place sorting, and the Dutch National Flag algorithm.

"🔗 Solve on LeetCode → Problem 75: Sort Colors" (https://leetcode.com/problems/sort-colors/description/)

"Sort Colors Example" (sort-colors-example.png)

📌 Problem Statement

Given an integer array "nums" containing only "0", "1", and "2", sort the array in-place so that all "0"s appear first, followed by "1"s and then "2"s.

Example

Input:  [2, 0, 2, 1, 1, 0]
Output: [0, 0, 1, 1, 2, 2]

Constraint: Do not use the built-in sorting function.

💡 Approach 1: Counting Sort

Idea: Count the occurrences of each number, then overwrite the original array in sorted order.

Steps

1. Count the number of zeros, ones, and twos.
2. Fill the array with zeros.
3. Fill the next positions with ones.
4. Fill the remaining positions with twos.

Complexity Analysis

Complexity| Cost
Time| "O(n)"
Auxiliary Space| "O(1)"
Traversals| Two passes

📄 Code: "SortColorsBruteForce.java" (SortColorsBruteForce.java)

⚡ Approach 2: Dutch National Flag Algorithm

Idea: Use three pointers to sort the array in one pass.

Pointer| Purpose
"low"| Position for the next "0"
"mid"| Current element being checked
"high"| Position for the next "2"

Steps

1. If "nums[mid] == 0", swap it with "nums[low]", then increment "low" and "mid".
2. If "nums[mid] == 1", increment "mid".
3. If "nums[mid] == 2", swap it with "nums[high]", then decrement "high".
4. Repeat while "mid <= high".

Complexity Analysis

Complexity| Cost
Time| "O(n)"
Auxiliary Space| "O(1)"
Traversals| One pass

📄 Code: "SortColorsOptimal.java" (SortColorsOptimal.java)

🔍 Approach Comparison

Feature| Counting Sort| Dutch National Flag
Time Complexity| "O(n)"| "O(n)"
Auxiliary Space| "O(1)"| "O(1)"
Traversals| Two| One
In-place| Yes| Yes

🧠 Key Takeaways

- Counting is useful when the input contains a small, fixed set of values.
- Three pointers help divide the array into sorted regions.
- The Dutch National Flag algorithm achieves one-pass sorting with constant extra space.

🛠️ Concepts Practised

"Arrays" · "Two Pointers" · "Sorting" · "In-Place Algorithms" · "Time Complexity"

---

⭐ DSA Practice | Java | LeetCode #75
