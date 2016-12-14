# LeetCode-with-JS
solutions for leetcode problems(mainly Algorithm)

### 1. Two Sum
```
/**
 * @param {number[]} nums
 * @param {number} target
 * @return {number[]}
 */
var twoSum = function(nums, target) {
  var a = [];
  for (var i = 0, len = nums.length; i < len; i++) {
    var tmp = target - nums[i];
    if (a[tmp] !== undefined) return [a[tmp], i];
    a[nums[i]] = i;
  }
};
```
