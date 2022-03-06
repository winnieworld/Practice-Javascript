<div align="center">
<h3>
LeetCode_Longest Common Prefix
</h3>
</div>  
```
var longestCommonPrefix = function(strs) {
    let sampleCord=strs[0]; //일치하는 부분 i가업글 될때마다 리뉴얼 되어야 할 것!
    let answer=""
    for(let i=1; i<strs.length; i++){
        if(strs[i].length=="") return ""
        for(let j=0; j<strs[i].length ; j++){
            if(strs[i][0]!=sampleCord[0]) return ""
            if (strs[i][j]==sampleCord[j]){
                answer+=strs[i][j]
            }else if(answer.length!=0 || j==strs[i].length-1){ 
                sampleCord = answer
                answer = ""
                break               
            }
        }
        if(answer.length!=0){ 
            sampleCord=answer
            answer=""}
    }
    if(strs.length==1){return strs[0]}else{ return sampleCord}
};

```

```
