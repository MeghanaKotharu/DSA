Notes for reference

1.we should never move the head node of a LL futher if we do that we will be losing all the nodes at front.
    Instead we need to create an another pointer pointing to head an move it further and make changes or utilize elements etc.

2.The fast and slow pointers can be used to get the slow pointer to the middle element 
    What we will be doing is:

       1. We keep 2 pointers fast and slow at the head node
       2. We move the slow pointer by 1 step and fast pointer by 2 steps.
    So when the fast pointer reaches end, slow pointer be at the middle.

3.Two pointers technique is widely used in LL.




Floyd Warshall ALgorithm (Linked List cycle start node)
![](https://user-images.githubusercontent.com/70280546/166112578-7b523d14-5c66-4a02-bc4c-ae49169c68ee.png)
[Reference Link](https://leetcode.com/problems/linked-list-cycle-ii/discuss/44774/Java-O(1)-space-solution-with-detailed-explanation.)
