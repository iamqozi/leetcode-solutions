# 1. Two Sum

**Problem:** https://leetcode.com/problems/two-sum/  
**Status:** Not started — the C++ file is an unfinished starter.

## Goal

Find two distinct positions whose values add up to the target.
Read the complete statement and constraints on LeetCode.

## First attempt

Start by thinking about every pair of positions.

- How can you avoid pairing a position with itself?
- How can you avoid checking the same pair twice?
- Should you return the values or their positions?

Try writing that approach before reading the optional hint.

<details>
<summary>Optional hint for improving the approach</summary>

For each value, calculate the value needed to reach the target.
Think about how you could quickly find that needed value among items
already visited, while also keeping its position.

</details>

## Practice example

For `nums = [3, 2, 4]` and `target = 6`, the positions are `[1, 2]`.
C++ vector indices start at zero.

## My explanation

After solving, use [the explanation template](../../templates/explanation.md)
to record the approach, complexity, checked cases, and what you learned.

## Submission

Not submitted. Replace the starter body before submitting on LeetCode.
