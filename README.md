# LeetCode-287-Find-the-Duplicate-Number.
Given an array nums of length n+1 where each value is between 1 and n, exactly one number appears twice. Return that duplicate without modifying the array and using only constant extra space.

# LC287 – Find the Duplicate Number

## Problem Statement
Given an integer array `nums` containing _n + 1_ integers where each integer is in the range `[1, n]` inclusive, there is only **one** repeated number in `nums`. Return this repeated number without modifying the array and using only constant extra space.

### Examples

Input: nums = [1,3,4,2,2]
Output: 2

Input: nums = [3,1,3,4,2]
Output: 3


## Approach
1. **Frequency Array (O(n) space)**  
   - Create a fixed-size `visit[]` of length `n + 1` initialized to `0`.  
   - Iterate through `nums`, for each `x = nums[i]`, check `visit[x]`:  
     - If it’s `0`, mark `visit[x] = 1`.  
     - Otherwise, you’ve found the duplicate — return `x`.

2. **(Note: For true O(1) space, Floyd’s Tortoise and Hare cycle detection can be used.)**

