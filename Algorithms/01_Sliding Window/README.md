In sliding window always the j-i+1 will be the size of the window(if j moves faster than i).

**Fixed size sliding window motto**
1.first reach the size of the window(k) by incrementing j and adding elements as per condition
         if  (j-i+1)==k  --> window size was reached, bez indexing starts from 0.
2. once window size was reached add one element and remove start element if it previously satisfied condition (Increment i and j ).
![image](https://user-images.githubusercontent.com/70280546/167442386-b35eee15-dd7d-4370-b84a-e03c5afc3187.png)


