# 🧩 Array Patterns

**Don't memorize every solution. Learn to recognize the pattern!**

## ⚡ The 4 Patterns at a Glance

### 1. Two Pointers 👈 👉

**Think:** Can two positions help me eliminate unnecessary comparisons?

- **Use for:** Pairs in sorted arrays, palindrome checks, removing duplicates.
- **Example:** Find two numbers adding up to `9` in `[2, 7, 11, 15]`.
- **Why it works:** Move pointers based on the sum instead of checking every pair.
- **Remember:** Sorted order matters for the usual target-sum technique.

### 2. Sliding Window 🪟

**Think:** Am I working with a continuous section of an array or string?

- **Use for:** Maximum sum of a fixed-size subarray, longest valid substring.
- **Example:** Find the maximum sum of any 3 consecutive elements.
- **Why it works:** Reuse the previous window's result as the window moves.
- **Remember:** Be careful with negative numbers and the condition used to shrink a variable-size window.

### 3. Kadane's Algorithm 📈

**Think:** What's the maximum sum of a contiguous subarray ending here?

- **Use for:** Maximum subarray sum.
- **Example:** `[-2, 1, -3, 4, -1, 2, 1]` → maximum sum is `6`.
- **Why it works:** Extend the current subarray or start a new one, whichever is better.
- **Remember:** Handle all-negative arrays correctly.

### 4. Prefix Sum ➕ 

**Think:** Can cumulative sums help me answer range-sum questions quickly?

- **Use for:** Range sums and some subarray-sum problems.
- **Example:** `[2, 4, 1, 3]` → prefix sums `[2, 6, 7, 10]`. Sum of indices `1–3` is `10 - 2 = 8`.
- **Why it works:** Subtract the sum before a range from the cumulative sum at its end.
- **Remember:** Keep indexing consistent.

---

## 🎯 Which Pattern Should I Try?

| Problem clue | Pattern |
|---|---|
| Sorted array, pair or opposite ends | Two Pointers |
| Continuous range, longest or shortest | Sliding Window |
| Maximum contiguous subarray sum | Kadane's Algorithm |
| Cumulative totals or range sums | Prefix Sum |

## 🧠 My Problem-Solving Checklist

- [ ] Understand the input and constraints.
- [ ] Try brute force when useful.
- [ ] Identify the pattern and explain why it works.
- [ ] Check edge cases.
- [ ] Compare time and space complexity.

*Learning DSA one problem, one pattern, and one improvement at a time.* 🚀
