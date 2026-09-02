# 01 — Hashing & Recursion Basics

Foundational Python DSA practice covering digit manipulation, divisor-finding, hashing/frequency patterns, and an end-to-end recursion progression.

**Notebook:** `01-hashing-and-recursion-basics.ipynb`

---

## Contents

### 1. Digit Manipulation
| Problem | Concept |
|---|---|
| Count digits in a number | Repeated integer division (`// 10`) |
| Reverse a number | Extract last digit (`% 10`), rebuild in reverse |
| Armstrong number check | Sum of `digit^n` where `n` = number of digits |

**Key idea:** any digit-by-digit problem reduces to a `while num > 0` loop using `% 10` (extract) and `// 10` (shift).

### 2. Finding Divisors
| Approach | Complexity | Notes |
|---|---|---|
| Brute force — check every `i` up to `n` | O(n) | Simple but slow for large `n` |
| Optimized — check up to `√n`, add both `i` and `n/i` | O(√n) | Standard divisor-finding pattern; avoids duplicate when `i == n/i` |

**Key idea:** divisors pair up around `√n` — if `i` divides `n`, so does `n/i`. Checking only up to `√n` and collecting both halves cuts the work from linear to square-root time.

### 3. Hashing & Frequency Counting
| Problem | Technique |
|---|---|
| Frequency of elements in a list | Dictionary hashing with `.get(key, 0) + 1` |
| Count occurrences of query elements in an array | Brute-force nested loop (O(n·m)) vs. **precomputed hash array** (O(n + m)) |
| Frequency using a fixed-size list instead of a dict | Direct-address table (index = value) |
| Character frequency in a string, filtered by a query list | Dictionary hashing on characters |

**Key idea — the core hashing pattern:** precompute frequencies once into a hash structure (dict or array), then answer any number of queries in O(1) each, instead of re-scanning the data every time. This is the single biggest optimization jump in the notebook — going from checking each query against the whole array (slow) to a single pass that builds a lookup table (fast).

### 4. Recursion — Building Intuition
| Problem | What it teaches |
|---|---|
| Simple function call | Baseline — no recursion yet |
| Recursion with a **global variable** and a depth limit | Shows why relying on global state is fragile — prefer passing state through parameters |
| Print numbers `i` to `n` (print **before** the recursive call) | Pre-order recursion — executes top-down |
| Print numbers `i` to `n` (print **after** the recursive call) | Post-order recursion — executes bottom-up (unwinds in reverse) |
| Print `n` down to `1` | Recursion without an accumulator |
| Sum of 1 to N (accumulator passed as parameter) | Tail-recursion style — carrying state forward instead of relying on return values |
| Sum of 1 to N (using return value) | Classic recursive accumulation — `n + func(n-1)` |
| Factorial of N | Same pattern as sum, with multiplication |

**Key idea:** the position of your logic (before vs. after the recursive call) determines execution order. Before = top-down. After = bottom-up (stack unwinds first).

### 5. Recursion on Arrays & Strings
| Problem | Technique |
|---|---|
| Reverse an array — **iterative** | Two-pointer swap (`left`, `right` converge) |
| Reverse an array — **recursive** | Same two-pointer idea, expressed as a recursive call instead of a loop |
| Palindrome check | Recursive two-pointer comparison; base case when pointers cross |

**Key idea:** two-pointer logic (converging `left`/`right` indices) translates directly into recursion — each recursive call is one "step" the loop would have taken.

### 6. Recursion — Fibonacci (OOP style)
| Problem | Technique |
|---|---|
| Nth Fibonacci number | Classic recursive branching: `fib(n) = fib(n-1) + fib(n-2)`, implemented as a class method |

**Key idea:** first exposure to *branching* recursion (two recursive calls per invocation) rather than the single-call recursion used everywhere else in this notebook — this is also the first place where the naive approach is exponential time, motivating memoization/DP later in the learning path.

---

## What's next in this path
- Memoized Fibonacci (top-down DP) → transition into Dynamic Programming
- Binary search (divide-and-conquer, a different recursion shape)
- Sliding window & two-pointer problems as their own category
- Sorting algorithms implemented from scratch

See the [root README](../README.md) for the full learning path and progress tracker.
