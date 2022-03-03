<div align="center">
<h3>
MostAppearNumber
</h3>
</div>  
```
function solution(s) {
    let arr=s.split("")
    let answer =new Array(9).fill(0)
    let max=0;
    let x=0;
    for (let i=0; i<arr.length; i++){
        answer[arr[i]]+=1;
    }
    for(let i =0; i<answer.length; i++){
       if (max<answer[i]){max =answer[i]
       x=i}
    }
    return x
}
```
