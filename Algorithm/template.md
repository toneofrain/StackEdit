### 1. [leetcode #937 Reorder Data in Log Files](https://leetcode.com/problems/reorder-data-in-log-files/) 

### 2. 처음 풀이

``` python
class Solution(object):
    def reorderLogFiles(self, logs):
        """
        :type logs: List[str]
        :rtype: List[str]
        """
        
        letter_logs = [log for log in logs if log.split()[1].isalpha()]
        digit_logs = [log for log in logs if log.split()[1].isdigit()]
        
        letter_logs.sort(key=lambda x: (x.split()[1:], x.split()[0]))        
        letter_logs.extend(digit_logs)
        
        return letter_logs
```

### 3. 문제점 / 해결책

### 4. 레퍼런스 코드

### 5. 최종

``` python

```

### 6. 파이썬
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTU3MjA0NzI4OSwxNTcyMDQ3Mjg5LDczMD
k5ODExNl19
-->