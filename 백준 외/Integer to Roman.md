<div align="center">
<h3>
LeetCode_Integer to Roman
</h3>
</div>  
```
var intToRoman = function(num) {
  
  let answer="";
  let x =0
   if(num/1000>=1){
       x = Math.floor(num/1000)
       answer += "M".repeat(x)
       num-=x*1000
   }     
   if(Math.floor(num/100)==9||Math.floor(num/100)==4){
    x = Math.floor(num/100)
    if (x==9){
        answer += "CM"
        num-=900
    } else if (x==4){
        answer+= "CD"
        num-=400

    }

}

else if(num/500>=1){
x = Math.floor(num/500)
answer += "D".repeat(x)
num-=x\*500

}
if(num/100>=1){
x = Math.floor(num/100)
answer += "C".repeat(x)
num-=x\*100

}
if(Math.floor(num/10)==9||Math.floor(num/10)==4){
x = Math.floor(num/10)
if (x==9){
answer += "XC"
num-=90

    } else if (x==4){
        answer+= "XL"
        num-=40
    }

}
else if(num/50>=1){
x = Math.floor(num/50)
answer += "L".repeat(x)
num-=x\*50

} if(num/10>=1){
x = Math.floor(num/10)
answer += "X".repeat(x)
num-=x\*10
}

if(Math.floor(num/1)==9||Math.floor(num/1)==4){
x = Math.floor(num/1)
if (x==9){
answer += "IX"
num-=9
} else if (x==4){
answer+= "IV"
num-=4
}

}
else if(num/5>=1){
x = Math.floor(num/5)
answer += "V".repeat(x)
num-=x\*5

}
if(num/1>=1){
x = Math.floor(num/1)
answer += "I".repeat(x)
num-=x\*1

}
return answer
};

```

```
