# Who Will Win

Solved on **GFG** · Difficulty: **Unknown** · Category: **Binary Search**

[View problem](https://www.geeksforgeeks.org/problems/who-will-win-1587115621/)

## Solution

```python
class Solution:
    def binarySearch(self, arr, k):
        # code here
        
        low = 0
        high = len(arr) - 1

        while low <= high:
            mid = low + (high - low) // 2

            if arr[mid] == k:
                return True

            elif arr[mid] < k:
                low = mid + 1

            else:
                high = mid - 1

        return False
```
