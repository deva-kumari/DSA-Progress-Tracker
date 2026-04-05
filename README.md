# Sliding Window Maximum (LC 239)

## Problem
Given an array of integers and a window size k, return the maximum element in each sliding window.

---

## Approach
We use a deque to maintain indices in decreasing order.

- Remove indices out of window
- Remove smaller elements from back
- Front always stores maximum

---

## Why This Approach
Brute force is O(n*k).  
Using deque → O(n)

---

## How It Works
- Maintain decreasing order
- Store indices instead of values
- Use front for max

---

## Real Life Example
Finding highest temperature in last k days.

---

## Pattern
Sliding Window + Monotonic Queue

---

## Complexity
Time: O(n)  
Space: O(k)
