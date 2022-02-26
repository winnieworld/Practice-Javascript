<div align="center">
<h3>
DefenseCastle
</h3>
</div>  
```
function solution(distance, time) {
    let come=[]
    let tmp=0;
    for(let i =0; i<distance.length; i++){
        come.push(distance[i]/time[i])
    }
    let we=0; //아군
    let bad=0;//적군
    let count =0;
    come.forEach(element=>{        
        come.forEach(name=>{
            if (element==name) count++
        })
        if(element<count) return -1 
    we=element
    bad=count
    })
   if(we-come.length<0) {return -1}else{return we-come.length} 
}
```
