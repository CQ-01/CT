### 비교연산
```py
A, B = map(int,input().split())
if (A - B) > 0:
    print('>')
elif (A - B) < 0:
    print('<')
else:
    print('==')
```
- input() : 입력 시 str로 받음

```py
pt = int(input('시험점수를 입력하세요 :'))
if pt >= 90:
    print('A')
elif pt >= 80:
    print('B')
elif pt >= 70:
    print('C')
elif pt >= 60:
    print('D')
else:
    print('F')
```
- input 내의 텍스트를 지워야 정답으로 인정됨..?