<div align="center">
<h3>
leetcode_Search in Rotated Sorted Array
</h3>
</div>

```
var search = function(nums, target) {
    let answer=-1;
    nums.forEach((element,index)=>{
        if(element==target){
            answer=index
        }
    })
  return answer==-1?  -1 :  answer
};
```
