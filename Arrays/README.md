# Shortest Distance to Target String in a Circular Array (LC 2515)

## Problem
You are given a circular array of strings and a target string.  
Starting from a given index, you can move left or right.  
Return the minimum number of steps required to reach the target.

If target does not exist, return -1.

---

## Approach

We iterate through the array and check all indices where the target exists.

For each index:
- Calculate clockwise distance
- Calculate anti-clockwise distance
- Take the minimum

---

## Why This Approach?

Since the array is circular:
- Moving beyond end comes back to start
- Moving before start goes to end

So we use modulo arithmetic.

---

## How It Works

For index `i`:
- Clockwise = (i - startIndex + n) % n
- Anti-clockwise = (startIndex - i + n) % n

Take minimum of both.

---

## Example

Input:
words = ["hello","i","am","leetcode","hello"]  
target = "hello"  
startIndex = 1  

Output:
1

---

## Pattern

Circular Array + Minimum Distance

---

## Complexity

Time: O(n)  
Space: O(1)
