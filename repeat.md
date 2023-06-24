### 구구단
```py
N = int(input())
for i in range (1, 10):
    print(N, '*', i, '=', N * i)
```
- 표시형식 고민

### 입력횟수만큼 반복
```py
T = int(input())
for i in range(T):
    A, B = map(int, input().split())
print(A + B)
```
- for i in range(T) : T 만큼 반복
- for i in range(1, T) : 1 ~ T-1 만큼 반복

### 반복합
```py
n = int(input())
a = 0
for i in range(1, n+1):
    a = a + i
print(a)
```

### 가격 합계
```py
X = int(input())
N = int(input())
n = 0
for i in range(N):
    a, b = map(int, input().split())
    n = n + (a * b)
if X == n:
    print('Yes')
else:
    print('No')
```
- n을 for문 안에 넣었다가 헤맴

### 한줄에서 출력반복
```py
N = int(input())
if N % 4 == 0:
    for i in range(N // 4):
        print('long', end=' ')
    print('int')
else:
    for i in range(N // 4+1):
        print('long', end=' ')
    print('int')
```
- print(end='') : 반복출력시 출력 구분자 설정
- 두 경우 합친 코드 생각
- gpt 참고 코드
```py
N = int(input())
long_count = N // 4
remainder = N % 4

for _ in range(long_count):
    print('long', end=' ')

if remainder != 0:
    print('long', end=' ')
print('int')
```
