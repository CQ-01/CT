```py
# 덧셈 계산
print(sum(list(map(int,input().split()))))
```

- list() : sum을 적용하기 위해 리스트로 변환
- map() : 숫자를 정수로 변환
- int, : map에서 최소 2개의 인자가 필요
<br><br/>
```py
# 뺄셈 계산
A, B = map(int,input().split())
print(A - B)
```
- 곱셈 나눗셈 계산도 같음

```py
# 세자리 수의 곱셈
A = int(input())
B = input()
b1 = int(B[0])
b2 = int(B[1])
b3 = int(B[2])
B = int(B)
print(A*b3)
print(A*b2)
print(A*b1)
print(A*B)
```

```py
# 특수문자 출력
print("\\    /\\")
print(" )  ( ')")
print("(  /  )")
print(" \\(__)|")
```
- `\\` : 이스케이프