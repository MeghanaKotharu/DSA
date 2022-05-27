Notes for reference

1.we should **never move the head node of a LL** futher if we do that we will be losing all the nodes at front.
    
Instead we need to create an another pointer pointing to head an move it further and make changes or utilize elements etc.

2.**The fast and slow pointers** can be used to get the slow pointer to the middle element 
    What we will be doing is:

       1. We keep 2 pointers fast and slow at the head node
       2. We move the slow pointer by 1 step and fast pointer by 2 steps.
    So when the fast pointer reaches end, slow pointer be at the middle.

3.Two pointers technique is widely used in LL.

4.Whenever you need to **delete a node but didn't have the previous node.**
    Replace the value of current node with the next node and change the reference of current node to current.next.next

5.      ListNode res=new ListNode();       //creates an empty node(not LL)
        ListNode head=res;                 //refers to a node
        
6.Suppose temp=head then:

        temp=temp.next              //will move the temp variable to next it won't delete anything.
        temp.next=temp.next.next    //removes the next node of temp.
    Changing the address of temp.next will remove next element.

7.Sometimes **Instead of creating a new list for result** we can simply:

       1.Create a dummy node.
       2.Keep a reference pointer to dummy node
       3.Now add elements one by one from given condition according to qn.
       
       
       ListNode dummy = new ListNode(0);   //O(1)   -->Step1
       ListNode curr = dummy;              //O(1)   -->Step2
[Merge LL](https://github.com/MeghanaKotharu/DSA/blob/main/DataStructures/LinkedList/Easy/03.%20Merge%202%20sorted%20Lists)

8.You can **store the previous node also sometimes**:

        1.Create a dummy node add it to head make it head and prev
        2.Curr will be referring to head.next 
        2.You need to update previous only when condition is not satisfied.
        
 See second approach.
[Remove elements in LL](https://github.com/MeghanaKotharu/DSA/blob/main/DataStructures/LinkedList/Easy/05.%20Remove%20elements%20in%20ll)

9.When you want to **access the adjacent elements to head(say 2) and remove both of them.**
you can increment head only once when the condition is not satisfied
[Remove Duplicates](https://leetcode.com/problems/remove-duplicates-from-sorted-list/discuss/28614/My-pretty-solution.-Java.)

10.It's mandatory to always check whether our solution works for odd and even LL

11.While moving the f-s pointers Incase of even no of nodes in LL the fast pointer won't reach the last element so we check the condition for fast.next.next!=null
     1->2->2->1     then fast will end at 2 and we shouldn't move it to 2.next.next as there is null
     for odd    1->2->->2->1->3     then fast will reach 3 and stops as fast.next==null
   
12.When you **reverse a LL** at last don't forget to change the head of a LL to previous otherwise it will refer to last element only.[Reverse a LL](https://github.com/MeghanaKotharu/DSA/blob/main/DataStructures/LinkedList/Easy/7.Reverse%20a%20LL)



Floyd Warshall ALgorithm (Linked List cycle start node)
![](https://user-images.githubusercontent.com/70280546/166112578-7b523d14-5c66-4a02-bc4c-ae49169c68ee.png)
[Reference Link](https://leetcode.com/problems/linked-list-cycle-ii/discuss/44774/Java-O(1)-space-solution-with-detailed-explanation.)
