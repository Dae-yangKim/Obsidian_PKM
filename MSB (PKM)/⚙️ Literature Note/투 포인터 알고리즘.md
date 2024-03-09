
---
- author : Daeyang-Kim
- created : 2024-02-13 22:55
- last_updated : 2024-02-13 22:55
- tags : #Literature #Algorithm
---

# 투 포인터 알고리즘

## *주제*

투 포인터 알고리즘에 대해서 정리

## *정리*

``` python

n = 5
m = 5

count = 0
interval_sum = 0
e = 0

for s in range(n):
	while interval_sum < m and e < n:
		interval_sum += data[e]
		e += 1

	if interval_sum == m:
		count += 1
	interval_sum -= data[s]

print(count)

```

리스트에 순차적으로 접근해야 할 경우 , _두 점의 위치를 기록하면서 처리하는 알고리즘_ 이다.

시간 복잡도 : O(N)

<b><mark>설명</mark></b>

start = 0 , end = 0 이렇게 처음 리스트의 부분을 start , end로 초기화

해당 인덱스의 리스트의 합이 target보다 작다면 end를 증가
start ~ end 사이의 합이 만약 <mark>target보다 작지 않다면 target과 동일한지 확인</mark>

동일하지 않다면 , start부분만큼 합에서 빼고 , start를 증가
같다면 count를 증가시킨다.

이렇게 한다면 해당 리스트 안에서 target값을 조합할 수 있는 수가 몇개 있는지 파악 가능.

## *참고문헌*

- [https://butter-shower.tistory.com/226](https://butter-shower.tistory.com/226)

---

## *Link*
