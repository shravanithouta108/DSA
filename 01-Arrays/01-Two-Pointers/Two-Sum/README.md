# 🔍 LeetCode 167: Two Sum II – Input Array Is Sorted

**Topic:** Arrays · Two Pointers <br>
**Difficulty:** Medium <br>
**Language:** Java

[🔗 View Problem on LeetCode](https://leetcode.com/problems/two-sum-ii-input-array-is-sorted/)

## 🎯 Problem

Given a **sorted array**, find two numbers that add up to `target`. Return their **1-based indices**.

**Example**

```text
numbers = [2, 7, 11, 15]
target = 9
Output = [1, 2]
```

## 👣 Trace the Two Pointers

Start with `left = 0` and `right = 3`.

| Step | Left | Right | Sum | Decision |
|---|---:|---:|---:|---|
| 1 | 2 | 15 | 17 | Too large → move `right` left |
| 2 | 2 | 11 | 13 | Too large → move `right` left |
| 3 | 2 | 7 | 9 | Match! Return `[1, 2]` |

*The table shows array values; the Java pointers start at zero-based positions. The returned indices are 1-based.*

## 💡 Approach 1: Brute Force

Check every possible pair using two loops.

- **Time:** `O(n²)`
- **Extra space:** `O(1)`

Code: [`TwoSumBruteForce.java`](TwoSumBruteForce.java)

## ⚡ Approach 2: Two Pointers

1. Place `left` at the beginning and `right` at the end.
2. If the sum is too small, move `left` forward.
3. If the sum is too large, move `right` backward.
4. If the sum matches the target, return both indices.

- **Time:** `O(n)`
- **Extra space:** `O(1)`

Code: [`TwoSumOptimal.java`](TwoSumOptimal.java)

## 🧠 Remember Before Solving

- **Sorted array?** Consider two pointers.
- **Sum too small?** Move `left` right to increase the sum.
- **Sum too large?** Move `right` left to decrease the sum.
- **Found the target?** Return `left + 1` and `right + 1`.
- **Why is it efficient?** Each pointer moves in only one direction, so we avoid checking every pair.

**Key takeaway:** Brute force checks pairs one by one. Two pointers use the sorted order to solve the problem in linear time. 🚀
