```python
import numpy as np

def solution(board, moves):
    board=np.array(board)
    answer = 0
    stack=[]
    j=0
    for i in moves:
        chosen=board[:,i-1]  
        for j in range(len(chosen)): 
            if chosen[j]!=0:
                stack.append(chosen[j])
                chosen[j]=0
                for k in range(1,len(stack)):
                    if stack[k]==stack[k-1]:
                        del stack[k-1:k+1]
                        answer+=2
                break
    return answer
```

