# Codess
Code for Certication in Machine Learning, UI/UX and DSA

#DSA

Assignment 1 - LeetCode 493

Reverse Pairs

Given an integer array, count all reverse pairs where nums[i] > 2 * nums[j] and i < j.
Approach: Modified Merge Sort. During the merge step, both halves are already sorted — so two pointers are used to count valid pairs in O(n) per level instead of checking every combination.

Time: O(n log n) | Space: O(n)

Key insight: Counting and merging are done as separate steps. Count pairs first using two pointers on sorted halves, then do the normal merge.

Assignment 2 - LeetCode 142

Linked List Cycle II 

Detect the node where a cycle begins using Floyd's Two-Pointer algorithm. Phase 1 detects cycle existence. Phase 2 uses the mathematical property F = C - a to find the exact start node by moving pointers from head and meeting point simultaneously.


Time: O(n) | Space: O(1)

Assignament 3 - LeetCode 2952


Minimum Number of Coins to Add 


Greedy approach using a reach variable. Sort coins, then iterate — if the current coin fits within reach + 1, extend reach. If there's a gap, greedily add a coin of value reach + 1 to plug it. Repeat until reach covers the full target.


Time: O(n log n) | Space: O(1)
