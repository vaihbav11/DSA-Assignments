Given an integer array, count all reverse pairs where nums[i] > 2 * nums[j] and i < j.
Approach: Modified Merge Sort. During the merge step, both halves are already sorted — so two pointers are used to count valid pairs in O(n) per level instead of checking every combination.
Time: O(n log n) | Space: O(n)
Key insight: Counting and merging are done as separate steps. Count pairs first using two pointers on sorted halves, then do the normal merge.
