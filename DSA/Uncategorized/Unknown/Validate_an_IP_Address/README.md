# Validate an IP Address:-

Solved on **GFG** · Difficulty: **Unknown** · Category: **Uncategorized**

[View problem](https://www.geeksforgeeks.org/problems/validate-an-ip-address-1587115621/)

## Solution

```python
class Solution:
    def isValid(self, ip):

        parts = ip.split(".")
        
        # must have exactly 4 parts
        if len(parts) != 4:
            return False
        
        for part in parts:
            # part must not be empty
            if part == "":
                return False
            
            # must contain only digits
            if not part.isdigit():
                return False
            
            # convert to integer
            num = int(part)
            
            # check range 0-255
            if num < 0 or num > 255:
                return False
            
            # no leading zeros allowed (except '0')
            if part != str(num):
                return False
        
        return True
```
