
# Maximum Average Subarray I (LC 643)

## Problem
Given an integer array nums and an integer k, find a contiguous subarray of length k that has the maximum average.

---

## Approach
We use a fixed size sliding window.

- Calculate sum of first k elements
- Slide the window:
  - Add next element
  - Remove previous element
- Track maximum sum

---

## Why Sliding Window?
Brute force takes O(n*k).

Sliding window reduces it to O(n).

---

## How It Works
- Maintain a window of size k
- Update sum in constant time
- Keep track of maximum sum

---

## Real Life Example
Finding highest average temperature over last k days.

---

## Pattern
Sliding Window (Fixed Size)

---

## Complexity
Time: O(n)  
Space: O(1)
