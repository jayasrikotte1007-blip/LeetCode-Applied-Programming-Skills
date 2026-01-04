**Binary Search**
Given an array of integers nums which is sorted in ascending order, and an integer target, write a function to search target in nums. If target exists, then return its index. Otherwise, return -1.

You must write an algorithm with O(log n) runtime complexity.

Example 1:
Input: nums = [-1,0,3,5,9,12], target = 9
Output: 4
Explanation: 9 exists in nums and its index is 4

Example 2:
Input: nums = [-1,0,3,5,9,12], target = 2
Output: -1
Explanation: 2 does not exist in nums so return -1
 
Constraints:
1 <= nums.length <= 104
-104 < nums[i], target < 104
All the integers in nums are unique.
nums is sorted in ascending order.

**Approach**
Since the array is already sorted, we use Binary Search. We compare the target with the middle element. If it matches, we return the index. If the target is smaller, we search in the left half; if it is larger, we search in the right half. We repeat this until the target is found or the search space becomes empty.

**Time Complexity**
o(log n)
**Space Complexity**
o(1)
