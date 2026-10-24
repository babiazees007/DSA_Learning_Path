# DSA Learning Path

My Data Structures & Algorithms practice in **Python**, organised by topic. Every notebook explains the idea in plain words, then walks from the **brute-force** solution to the **optimal** one, with time / space complexity and a short "key takeaways" section at the end.

All notebooks were run top to bottom, so the outputs you see are real.

## Contents

| # | Notebook | Topics | Open in Colab |
|---|---|---|---|
| 01 | [Array Basics](01_Array_Basics.ipynb) | largest / second largest, sorted check, remove duplicates, rotate array (reversal trick), move zeros | [![Open](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/babiazees007/DSA_Learning_Path/blob/main/01_Array_Basics.ipynb) |
| 02 | [Array Hashing & Subarrays](02_Array_Hashing_and_Subarrays.ipynb) | linear search, union, missing number, Two Sum, Kadane's algorithm, stock buy/sell, rearrange by sign, longest consecutive sequence | [![Open](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/babiazees007/DSA_Learning_Path/blob/main/02_Array_Hashing_and_Subarrays.ipynb) |
| 03 | [Matrix](03_Matrix.ipynb) | traversal patterns, transpose, set matrix zeroes, rotate 90°, spiral order | [![Open](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/babiazees007/DSA_Learning_Path/blob/main/03_Matrix.ipynb) |
| 04 | [Binary Search](04_Binary_Search.ipynb) | iterative + recursive, lower / upper bound, insert position, floor & ceil, first / last occurrence, rotated array (with and without duplicates), minimum in rotated array | [![Open](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/babiazees007/DSA_Learning_Path/blob/main/04_Binary_Search.ipynb) |
| 05 | [3Sum & 4Sum](05_Two_Pointers_3Sum_4Sum.ipynb) | brute force → hashing → sort + two pointers | [![Open](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/babiazees007/DSA_Learning_Path/blob/main/05_Two_Pointers_3Sum_4Sum.ipynb) |
| 06 | [Bit Manipulation](06_Bit_Manipulation.ipynb) | binary conversion, complements, operators, XOR tricks, bit flips, single number, power set | [![Open](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/babiazees007/DSA_Learning_Path/blob/main/06_Bit_Manipulation.ipynb) |
| 07 | [Recursion & Backtracking](07_Recursion_and_Backtracking.ipynb) | subsets, subsequences with sum k (all / one / count), binary strings without consecutive 1s | [![Open](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/babiazees007/DSA_Learning_Path/blob/main/07_Recursion_and_Backtracking.ipynb) |
| 08 | [Singly Linked List](08_Singly_Linked_List.ipynb) | insert / delete, middle node, reverse, cycle detection (start + length), odd-even list, remove N-th from end | [![Open](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/babiazees007/DSA_Learning_Path/blob/main/08_Singly_Linked_List.ipynb) |
| 09 | [Doubly Linked List](09_Doubly_Linked_List.ipynb) | full DLL class, reverse, remove all occurrences, pair sum, remove duplicates from sorted DLL | [![Open](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/babiazees007/DSA_Learning_Path/blob/main/09_Doubly_Linked_List.ipynb) |

> The Colab links assume the default branch is `main`.

## Patterns I practised

- **Two pointers**: remove duplicates, move zeros, 3Sum / 4Sum, pair sum in a sorted DLL
- **Hashing**: Two Sum, longest consecutive sequence
- **Kadane / running best**: max subarray, stock profit
- **Binary search on a sorted / rotated space**: bounds, rotated arrays
- **Slow & fast pointers**: middle node, cycle detection
- **Pick / not pick backtracking**: subsets and subsequences
- **Bit tricks**: XOR for single number, bitmask for subsets

## Running locally

```bash
pip install jupyter
jupyter notebook
```
