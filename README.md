# LeetCode 316 - Remove Duplicate Letters

## Problem Statement

Given a string `s`, remove duplicate letters so that every letter appears only once.

The result must be the **smallest possible string in lexicographical order** among all possible results.

## Example 1

### Input

```text
s = "bcabc"
```

### Output

```text
"abc"
```

## Example 2

### Input

```text
s = "cbacdcbc"
```

### Output

```text
"acdb"
```

## Approach

Use a **Greedy Approach with a Stack**.

Store the last occurrence of every character. While processing the string, remove a larger character from the stack if it appears again later, allowing a smaller character to come before it.

## Algorithm

1. Store the last occurrence of every character.
2. Create a stack to build the result.
3. Use a set to keep track of characters already in the stack.
4. Traverse the string from left to right.
5. Skip a character if it is already present.
6. While the current character is smaller than the stack's top character and the top character appears again later, remove the top character.
7. Add the current character to the stack.
8. Return the characters in the stack as a string.

## Time Complexity

`O(n)`

## Space Complexity

`O(n)`

## Key Concepts

* Greedy
* Stack
* Hash Set
* Last Occurrence
* Lexicographical Order
* String

## Language

Python

## LeetCode Details

* **Problem:** 316
* **Title:** Remove Duplicate Letters
* **Difficulty:** Medium

## Author

**T. Nandhini Reddy**

GitHub: `242t605119-dotcom`
