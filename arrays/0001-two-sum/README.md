# 1. Two Sum

**Problem:** https://leetcode.com/problems/two-sum/  
**Status:** Accepted — 65/65 test cases passed, confirmed by the submission screenshot.

## Approach

Use two loops to check every pair of distinct positions. The outer loop selects
index i. The inner loop starts at i + 1 and selects index j. If the two values
sum to the target, return their indices.

Starting j at i + 1 prevents using the same element twice and avoids checking
a pair again in reverse order. Every possible pair with i < j is considered,
so the guaranteed valid pair will be found.

## Walkthrough

For nums = [5, 8, 1, 3] and target = 9, indices 1 and 2 contain 8 and 1.
Since 8 + 1 = 9, return [1, 2].

## Complexity

- Time: O(n²) in the worst case, where n is the number of elements.
  At most n(n - 1)/2 pairs are checked.
- Extra space: O(1). Only loop indices and a fixed-size result are needed.

## Validation

LeetCode accepted the submitted approach on all 65 test cases.
The repository version includes <vector>, uses std::vector, and retains a
fallback empty return so every control path returns a value. The fallback
is not reached for inputs satisfying the problem's guarantee.

## Learning notes

Return indices rather than values. Two different indices may contain equal
values; it is the same element that cannot be used twice.

## Help and revisit

- Help used: Guided explanation and C++ code provided by ChatGPT.
- Independently revisited: Not yet.
- Next practice: Reimplement the nested-loop approach without looking at the code.
