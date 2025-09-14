# day-21-sort-0s-1s-2s
dutch flag algo
  void sort012(vector<int>& arr) {
         int n = arr.size();
        int low = 0, mid = 0 , high = n-1;
        
         while (mid <= high){
             if(arr[mid]==0){
                 swap(arr[low], arr[mid]);
                 low++;
                 mid++;
             }
             else if (arr[mid]== 1){
                 mid++;
              }
             else {
               swap( arr[mid] , arr[high]);
               high--;
            }     
           }
         }
