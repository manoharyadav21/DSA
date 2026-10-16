# DSA Day 1 — Arrays Fundamentals

**Target:** Microsoft India Fresher SDE Preparation  
**Language:** C++  
**Study Time:** 5 Hours

---

## 1. Today's Goals

By the end of Day 1, you should understand:

1. What is an array?
2. Array indexing (0-based indexing).
3. Traversing an array using loops.
4. Finding the minimum and maximum elements.
5. Finding the sum of array elements.
6. Basic time complexity: `O(1)`, `O(n)`, `O(n²)`.
7. Solving beginner-level array problems independently.

---

## 2. Five-Hour Study Plan

### Hour 1: Array Fundamentals
- Understand what an array is.
- Learn indexing and accessing elements.
- Learn input and output in C++.
- Practice traversing arrays using `for` loops.

### Hour 2: Basic Array Operations
- Find the sum of array elements.
- Find the maximum element.
- Find the minimum element.
- Reverse an array.
- Understand each solution step by step.

### Hour 3: Time Complexity
- Understand `O(1)`, `O(n)`, and `O(n²)`.
- Count how many times a loop executes.
- Analyze the complexity of your array solutions.

### Hour 4: LeetCode Practice

Solve these problems in order:

1. [LeetCode 1480 — Running Sum of 1d Array](https://leetcode.com/problems/running-sum-of-1d-array/)
2. [LeetCode 1672 — Richest Customer Wealth](https://leetcode.com/problems/richest-customer-wealth/)
3. [LeetCode 217 — Contains Duplicate](https://leetcode.com/problems/contains-duplicate/)

Try each problem independently before looking at hints.

### Hour 5: Revision and Interview Practice
- Re-solve one problem without looking at your old code.
- Explain your approach in simple English.
- State the time and space complexity.
- Write down mistakes and corrections.
- Review all concepts learned today.

---

## 3. What Is an Array?

An array stores multiple values of the same data type under one variable name.

Example:

```cpp
int nums[5] = {10, 20, 30, 40, 50};
```

| Index | Value |
|---:|---:|
| 0 | 10 |
| 1 | 20 |
| 2 | 30 |
| 3 | 40 |
| 4 | 50 |

**Important:**
- Array indexing starts at `0` in C++.
- `nums[0]` gives `10`.
- `nums[2]` gives `30`.
- `nums[4]` gives `50`.
- Accessing an invalid index can cause errors.

---

## 4. Basic C++ Array Template

```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
    int n;
    cin >> n;

    vector<int> nums(n);

    for (int i = 0; i < n; i++) {
        cin >> nums[i];
    }

    for (int i = 0; i < n; i++) {
        cout << nums[i] << " ";
    }

    return 0;
}
```

**Example Input:**

```text
5
10 20 30 40 50
```

**Output:**

```text
10 20 30 40 50
```

---

## 5. Time Complexity — Basics

### `O(1)` — Constant Time

```cpp
cout << nums[0];
```

Accessing one element takes constant time.

### `O(n)` — Linear Time

```cpp
for (int i = 0; i < n; i++) {
    cout << nums[i];
}
```

The loop processes `n` elements.

### `O(n²)` — Quadratic Time

```cpp
for (int i = 0; i < n; i++) {
    for (int j = 0; j < n; j++) {
        cout << nums[i] << " " << nums[j];
    }
}
```

Two nested loops each run `n` times, resulting in approximately `n × n` operations.

**Remember:** Always consider how the number of operations grows when the input size increases.

---

## 6. LeetCode Practice

### Problem 1: LeetCode 1480

**Title:** Running Sum of 1d Array  
**Concept:** Prefix sum / running sum.

**Goal:** For every index, calculate the sum of all elements from index `0` to that index.

Example:

```text
Input:  [1, 2, 3, 4]
Output: [1, 3, 6, 10]
```

[Open Problem](https://leetcode.com/problems/running-sum-of-1d-array/)

### Problem 2: LeetCode 1672

**Title:** Richest Customer Wealth  
**Concept:** Arrays and nested loops.

**Goal:** Find the maximum total wealth among customers.

Example:

```text
Input: [[1, 2, 3], [3, 2, 1]]
Output: 6
```

[Open Problem](https://leetcode.com/problems/richest-customer-wealth/)

### Problem 3: LeetCode 217

**Title:** Contains Duplicate  
**Concept:** Arrays and hashing (a first look at hashing).

**Goal:** Return `true` if any value appears at least twice; otherwise return `false`.

Example:

```text
Input: [1, 2, 3, 1]
Output: true
```

[Open Problem](https://leetcode.com/problems/contains-duplicate/)

---

## 7. Rules for Today

1. Understand the problem before writing code.
2. Write your own approach first.
3. Try solving independently for 20–30 minutes.
4. Test your code with multiple inputs.
5. Explain why your solution works.
6. Learn the time and space complexity.
7. Do not memorize solutions without understanding them.

---

## 8. End-of-Day Checklist

- [ ] I understand arrays and indexing.
- [ ] I can input and print an array in C++.
- [ ] I can traverse an array using a loop.
- [ ] I can find the minimum and maximum.
- [ ] I understand `O(1)`, `O(n)`, and `O(n²)`.
- [ ] I attempted all three LeetCode problems.
- [ ] I can explain my approach without reading code.

### Day 1 Success Criterion

Focus on understanding and independent problem-solving, not on solving as many problems as possible.

**Next: Day 2 — Array Problem-Solving Patterns**
