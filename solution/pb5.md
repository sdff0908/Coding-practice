```python
def solution(s):
    answer = True
    if len(s)!=4 and len(s)!=6 or s.isdigit()==False: 
        answer=False
    return answer
```

```bash
#isdigit:문자열 내에 숫자가 있는지?
#isalpha:문자열 내에 문자(한글,알파벳 등)가 있는지?
```