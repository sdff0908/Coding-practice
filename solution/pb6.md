```python
def solution(n):
    answer=-1                    #True개수=소수 개수, 1은 제외
    numList=[True]*n             #boolean 사용하면 시간 단축가능
    for i in range(2,n+1):
        for j in range(i+i,n+1,i):
            numList[j-1]=False
    answer+=numList.count(True)       
    return answer
```

