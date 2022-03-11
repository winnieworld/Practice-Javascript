<div align="center">
<h3>
LeetCode_Implement strStr()
</h3>
</div>  
```
var strStr = function(haystack, needle) {
    if (needle==""){return 0 }
    else if(haystack.includes(needle)){
        return haystack.indexOf(needle)
    } else{ return -1}
}

```

```
