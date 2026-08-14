# 🚀 LeetCode Journey — Day 1

My daily LeetCode practice repository for improving **Data Structures & Algorithms** using **C++**.

---

# 📌 Problem 1: Two Sum

* **Platform:** LeetCode
* **Difficulty:** Easy
* **Language:** C++

## 📝 Problem Statement

Given an integer array `nums` and an integer `target`, return the **indices** of the two numbers such that they add up to the target.

**Example**

```text
Input:
nums = [2,7,11,15]
target = 9

Output:
[0,1]
```

---

## 💡 My Approach (Brute Force)

I used a **nested loop** approach:

1. Pick one element using the outer loop.
2. Compare it with every following element.
3. If their sum equals the target, return both indices immediately.

This checks every possible pair until the correct answer is found.

---

## ⚙️ Solution

```cpp
class Solution {
public:
    vector<int> twoSum(vector<int>& nums, int target) {

        for (int i = 0; i < nums.size(); i++) {
            for (int j = i + 1; j < nums.size(); j++) {

                if (nums[i] + nums[j] == target) {
                    return {i, j};
                }
            }
        }

        return {};
    }
};
```

---

## ❓ Why is there no `main()`?

LeetCode already provides the `main()` function internally.

When you submit, LeetCode automatically creates an object of the `Solution` class and calls your `twoSum()` function with the test cases.

So we only write the required function—not because of OOP, but because it's the format LeetCode expects.

---

## ⏱️ Complexity Analysis

| Complexity | Value |
| ---------- | ----- |
| **Time**   | O(n²) |
| **Space**  | O(1)  |

---

## 📚 Concepts Practiced

* Vectors (`vector<int>`)
* Nested `for` loops
* Array traversal
* Index-based access
* Conditional statements
* Returning vectors (`return {i, j}`)

---

## ✅ Progress

| Day   | Problem | Difficulty | Status      |
| ----- | ------- | ---------- | ----------- |
| Day 1 | Two Sum | Easy       | ✅ Completed |

---

### 🎯 Goal

Solve LeetCode consistently, strengthen DSA fundamentals, and prepare for coding interviews and placements.

**Day 1 Complete ✅**
