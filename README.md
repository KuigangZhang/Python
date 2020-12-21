# Python
class Solution:
    def removeDuplicates(self, nums: List[int]) -> int:
        i = 0
        while i <= len(nums) - 2:
            if nums[i+1] != nums[i]:
                i += 1
            else:
                nums.remove(nums[i+1])
                i += 1

        return int(len(nums))
