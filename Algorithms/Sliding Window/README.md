In sliding window always the j-i+1 will be the size of the window(if j moves faster than i).

**Fixed size sliding window motto**

1.first reach the size of the window(k) by incrementing j and adding elements as per condition

         if  (j-i+1)==k  --> window size was reached, bez indexing starts from 0.
         
2. once window size was reached add one element and remove start element if it previously satisfied condition (Increment i and j ).


![image](https://user-images.githubusercontent.com/70280546/167444204-feac6cdf-ad5d-4127-a030-7429579c654c.png)

![image](https://user-images.githubusercontent.com/70280546/167444633-45250ffe-d235-4cc2-8130-ebbd962b9145.png)


![image](https://user-images.githubusercontent.com/70280546/167444645-fd7a55fb-2119-4284-abdb-f22307abcb9a.png)




