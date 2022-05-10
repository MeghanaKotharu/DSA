Reference of Questions: Aditya Verma Youtube Channel


**Binary Search in Descending order**
     
      private static int binarySearch(int[] a, int fromIndex, int toIndex, int key) {
        int start = fromIndex;
        int end = toIndex - 1;

        while (start <= end) {
            int mid = start + (end-start)/2;
            int midVal = a[mid];

            if (key < midVal)
                start = mid + 1;
            else if (key > midVal)
                end = mid - 1;
            else
                return mid; // key found
        }
        return -1;
    }
    
**Order Agnostic Binary Search (when we don't know in which order array is sorted)**


Just check any 2 elements in array to know if they are sorted in ascending order or not if ascending order search accordingly
else check incase of descending sorted array.
     
        private static int AgnosticbinarySearch(int[] a, int fromIndex, int toIndex, int key) {
        int start = fromIndex;
        int end = toIndex - 1;
        boolean isAsc= a[start] < a[end]
        while (start <= end) {
            int mid = start + (end-start)/2;
            int midVal = a[mid];

            if (key > midVal){
                if(isAsc) start = mid + 1; 
                else end = mid - 1;
            }
            else if (key < midVal){
                if(isAsc) end = mid - 1; 
                else start = mid + 1;
             }
            else
                return mid; // key found
        }
        return -1
     }
     
     
     
     
