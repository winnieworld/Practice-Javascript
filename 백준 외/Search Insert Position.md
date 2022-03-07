<div align="center">
<h3>
LeetCode_Search Insert Position
</h3>
</div>  
```
var searchInsert = function(nums, target) {
    nums.push(target);
    nums.sort((a, b) => a - b);
    return(nums.indexOf(target))
};
```
