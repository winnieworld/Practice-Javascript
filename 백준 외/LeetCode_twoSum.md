<div align="center">
<h3>
LeetCode_twoSum
</h3>
</div>  
<b>일부 오답</b>
 <br> traget값의 절반값이 있을때 해당 인덱스가 두번찍히는 오류가 있었다. 그래서 map으로 푸는가보다. map으로도 풀어보아야겠다.
```
var twoSum = function(nums, target) {
    let answer=[];
    for(let i=0; i<nums.length; i++){
        if(nums.includes(target-nums[i])&&nums.indexOf(target-nums[i]) !== i){
            answer.push(i)
            answer.push(nums.indexOf(target-nums[i]))
            return answer
        }
    
    }
    return answer
};
```
