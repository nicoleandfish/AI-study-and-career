##### 20240903 No2708. 一个小组的最大实力值
![image](https://github.com/user-attachments/assets/dded0a3b-e274-4240-bf93-6daa9806010e)
```
class Solution(object):
    def maxStrength(self, nums):
        neg = []
        pos = []
        
        for num in nums:
            if num < 0:
                neg.append(-num)
            if num > 0:
                pos.append(num)
        
        product = 1
        if len(pos) > 0:
            for num in pos:
                product *= num

        neg.sort()
        if len(neg) % 2 == 1:
            neg.pop(0) 
        
        for num in neg:
            product *= num

        if len(nums) == 1:
            product = nums[0]
        
        return product if product != 1 or (len(pos) > 0 or len(neg) > 0) else 0
```
