```python
def solution(n):
    answer=sum([div for div in range(1,n+1) if n%div==0])
    return answer
```

