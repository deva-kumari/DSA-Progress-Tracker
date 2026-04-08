# Count Good Substrings (LC 1876)

## Problem
Given a string s, return the number of substrings of length 3 with all distinct characters.

---

## Approach
We use sliding window of size 3.

- Expand window using right pointer
- Shrink using left pointer
- Use HashMap to track frequency
- If all characters are unique → count++

---

## Why Sliding Window?
Brute force checks all substrings → O(n*k)

Sliding window → O(n)

---

## How It Works
- Maintain window of size 3
- Add new character
- Remove old character
- Check if all characters are unique

---

## Real Life Example
Checking 3 people in a taxi:
If all are different → valid group

---

## Pattern
Sliding Window (Fixed Size)

---

## Complexity
Time: O(n)  
Space: O(1)
