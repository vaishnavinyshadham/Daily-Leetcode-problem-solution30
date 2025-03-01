# Daily-Leetcode-problem-solution30
PROBLEM

You are given a 0-indexed array nums of size n consisting of non-negative integers.
You need to apply n - 1 operations to this array where, in the ith operation (0-indexed), you will apply the following on the ith element of nums:
If nums[i] == nums[i + 1], then multiply nums[i] by 2 and set nums[i + 1] to 0. Otherwise, you skip this operation.
After performing all the operations, shift all the 0's to the end of the array.
For example, the array [1,0,2,0,0,1] after shifting all its 0's to the end, is [1,2,1,0,0,0].
Return the resulting array.
Note that the operations are applied sequentially, not all at once.

Approach

Apply the given operations sequentially:
If nums[i] == nums[i + 1], multiply nums[i] by 2 and set nums[i + 1] to 0.
Shift all zeros to the end:
Use the two-pointer approach to move non-zero elements to the front while maintaining order.
Fill the remaining elements with 0.

Edge Cases Handled

✅ All elements are zero (e.g., {0,0,0} → {0,0,0}).
✅ No adjacent duplicates (e.g., {1,2,3} → {1,2,3}).
✅ Single-element array (e.g., {5} → {5}).
✅ Already processed input

Time complexity:

Applying operations:
O(n)
Shifting non-zero elements:
O(n)
Overall complexity:
O(n) linear time.

Space complexity:

O(1) implies this is in place solution

 
