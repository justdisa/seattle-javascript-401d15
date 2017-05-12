Whiteboard DS Assignment: Find out of a singly linked list is circular:


This is the tortoise and hare algorithm. Create two pointers, one that moves forward one node at a time and one that moves forward two nodes at a time. While the two pointers are different, return false(no loop), and When they become the same, return true(loop).

```
function detectLoop(sll){
   var slowPointer = sll.head,
       fastPointer = sll.head;

   while(slowPointer && fastPointer && fastPointer.next){
     slowPointer = slowPointer.next;
     fastPointer = fastPointer.next.next;

     if(slowPointer == fastPointer){
        return true;
     }
   }
   return false;
}
```
Many thanks to [That JS Dude](http://www.thatjsdude.com/).
