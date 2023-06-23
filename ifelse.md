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

### 윤년 문제
```py
year = int(input())
if year % 4 == 0:
    if year % 100 != 0 or year % 400 == 0:
        print(1)
    else:
        print(0)
else:
    print(0)
```
- if 문마다 else로 받아줘야 함
- or의 활용 복기

### 좌표 사분면 문제
```py
x = int(input())
y = int(input())

if x > 0:
    if y > 0:
        print('1')
    elif y < 0:
        print('4')
elif x < 0:
    if y > 0:
        print('2')
    elif y < 0:
        print('3')
```
```py
x = int(input())
y = int(input())

if x > 0 and y > 0:
    print(1)
elif x < 0 and y > 0:
    print(2)
elif x < 0 and y < 0:
    print(3)
elif x > 0 and y < 0:
    print(4)
```
- 두 줄로 입력 이슈

### 시간 계산문제
```py
H, M = map(int, input().split())
time = (H * 60) + M
H2 = (time - 45) // 60
M2 = (time - 45) % 60
while H2 < 0:
    H2 = H2 + 24
print(H2, M2)
```

```py
H, M = map(int, input().split())
cook = int(input())
time = (H * 60) + M + cook
H2 = time // 60
M2 = time % 60
while H2 >= 24:
    H2 = H2 -24
print(H2, M2)
```
- 시간 넘어가는 문제 해결

### 주사위별 점수
```py
x1, x2, x3 = map(int,input().split())
if x1 == x2 == x3:
    print(10000 + x1 * 1000)
elif x1 == x2 or x1 == x3:
    print(1000 + x1 * 100)
elif x2 == x3:
    print(1000 + x2 * 100)
else:
    if x1 > x2 and x1 > x3:
        print(x1 * 100)
    elif x2 > x1 and x2 > x3:
        print(x2 * 100)
    elif x3 > x1 and x3 > x2:
        print(x3 * 100)
```
- max함수 이용하면 더 깔끔한 풀이