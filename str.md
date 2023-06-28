### 문자열 인덱스
```py
S = str(input())
i = int(input())
print(S[i-1])
```
### 문자열 길이
```py
S = str(input())
print(len(S))
```
### 문자열 인덱스2
```py
T = int(input())
for _ in range(T):
    text = str(input())
    print(text[0], end='')
    print(text[-1])
```
### 자릿수 덧셈
```py
int(input())
N = sum(map(int, str(input())))
print(N)
```
- `split()` 메서드는 리스트에서 사용불가

### 아스키코드
```py
S = list(str(input()))
ords = []
for _ in S:
    ords.append(ord(_))
for __ in range(97, 123):
    if __ in ords:
        print(ords.index(__), end=' ')
    else:
        print(-1, end=' ')
```
- `ord()` : 아스키코드 변환, 한개 요소만 받음

### 리스트 컴프리헨션
```py
N = int(input())
for _ in range(N):
    M, S = map(str, input().split())
    S = list(S)
    M = int(M)
    N_list = [__ for __ in S for ___ in range(M)]
    print(*N_list, sep='')
```
- `__ for __ in S for ___ in range(M)` : S내의 요소를 M번 반복
