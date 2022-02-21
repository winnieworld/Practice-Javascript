<div align="center">
<h3>
LeetCode_LinkedList
</h3>
</div>  
```
var swapPairs = function (head) {   
    let dummyList = new ListNode(null, head);
    function swapNodes(listNode) {        
        if (listNode && listNode.next && listNode.next.next) {            
            const first = listNode.next;
            const second = listNode.next.next;
          
            first.next = second.next;
            second.next = first;
            listNode.next = second;
            swapNodes(listNode.next.next);
        }
    }
    swapNodes(dummyList);
    return dummyList.next;
};
```
