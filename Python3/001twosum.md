Source: https://leetcode.com/problems/two-sum/

Author: Keisuke Yamada

Date: 2018-09-08

---
Given an array of integers, return indices of the two numbers such that they add up to a specific target.

You may assume that each input would have exactly one solution, and you may not use the same element twice.

Example:

Given nums = [2, 7, 11, 15], target = 9

Because nums[0] + nums[1] = 2 + 7 = 9

return [0,1]

---

    nums = [3,2,4]
    target = 6
        
    ans = []
    print(ans)
    flg = 0
    for i in range(len(nums)):
      if(flg==1):
        break
      for j in range(i+1,len(nums),1):
        if nums[i] + nums[j] == target:
          ans.append(i)
          ans.append(j)
          flg=1
          break

     print(ans)
