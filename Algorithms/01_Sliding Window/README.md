In sliding window always the j-i+1 will be the size of the window(if j moves faster than i).

**Fixed size sliding window motto**
1.first reach the size of the window(k) by incrementing j and adding elements as per condition
         if  (j-i+1)==k  --> window size was reached, bez indexing starts from 0.
2. once window size was reached add one element and remove start element if it previously satisfied condition (Increment i and j ).
![image](https://user-images.githubusercontent.com/70280546/167444204-feac6cdf-ad5d-4127-a030-7429579c654c.png)

![image](https://user-images.githubusercontent.com/70280546/167444323-51713296-d446-4fac-b992-666bf19968d7.png)

![image](https://user-images.githubusercontent.com/70280546/167444265-7b0267f8-9326-4caf-9633-e554d7002143.png)



