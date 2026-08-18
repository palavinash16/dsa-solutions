# Move All Negative Elements To End

Solved on **GFG** · Difficulty: **Unknown** · Category: **Uncategorized**

[View problem](https://www.geeksforgeeks.org/problems/move-all-negative-elements-to-end1813/)

## Solution

```cpp
class Solution {
  public:
    void segregateElements(vector<int>& arr) {
        // code here
        vector<int>ans;
        for(int i=0;i<arr.size();i++){
            if(arr[i]>0){
                ans.push_back(arr[i]);
            }
        }
        for(int i=0;i<arr.size();i++){
            if(arr[i]<0){
                ans.push_back(arr[i]);
            }
        }
        
        arr = ans;
    }
};
```
