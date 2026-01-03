**Sort-Colours**

Given an array nums with n objects colored red, white, or blue, sort them in-place so that objects of the same color are adjacent, with the colors in the order red, white, and blue.

We will use the integers 0, 1, and 2 to represent the color red, white, and blue, respectively.

You must solve this problem without using the library's sort function.

 

Example 1:

Input: nums = [2,0,2,1,1,0]
Output: [0,0,1,1,2,2]
Example 2:

Input: nums = [2,0,1]
Output: [0,1,2]
 

Constraints:

n == nums.length
1 <= n <= 300
nums[i] is either 0, 1, or 2.


**Approach**
Since the array has only three values (0, 1, and 2), I thought of counting how many times each value occurs. First, I loop through the array and count the number of 0s, 1s, and 2s. Then, I modify the same array by putting all the 0s first, followed by all the 1s, and then all the 2s. This way, the array gets sorted without using any built-in sorting function, and the logic is simple and easy to understand as a student.

**Time Complexity** 
O(n).
**Space Complexity**
O(1)
