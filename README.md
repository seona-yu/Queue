# Queue


# Queue(자료구조, 알고리즘) 

## 용도
**큐는 한쪽 끝에서만 자료를 넣고, 넣은 순서대로 뺄 수 있는 자료구조** 이다.
즉, 처음으로 저장된 데이터를 가장 먼저 사용하는 구조이다.

## 사용법

- **Push**
: **데이터를 차례대로 넣어 저장하는 것.** 

- **Get**
: **처음으로 저장된 데이터를 하나씩 사용하는 것.** 

## 예시 
### 파이썬으로 큐를 직접 구현. [백준 10845번 일부]
```    
import queue
que = queue.Queue()

n = int(input())
for i in range(0, n):
    a = input().split()
    if a[0]=="push":
        que.put(int(a[1]))
    elif a[0]=="pop":
        if que.qsize()==0:
            print(-1)
        else:
            print(que.get())
```
