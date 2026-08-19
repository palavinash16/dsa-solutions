# Check The Status

Solved on **GFG** · Difficulty: **Unknown** · Category: **Uncategorized**

[View problem](https://www.geeksforgeeks.org/problems/check-the-status/)

## Solution

```python
class Solution:
    def checkStatus(self, a, b, flag):
        # code here
        
        if flag:
            return a < 0 and b < 0
        else:
            return (a >= 0) != (b >= 0)  # Exactly one is non-negative
```
