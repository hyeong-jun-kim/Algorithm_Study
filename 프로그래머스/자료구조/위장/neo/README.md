## Info
<a href="https://school.programmers.co.kr/learn/courses/30/lessons/42578" rel="nofollow">위장</a>

## ❗ 풀이 방법
해당 문제는 DFS(백트래킹)을 사용해서 풀었다. 1번 문제를 제외하고 모든 테스트 케이스를 통과했다.

* 해당 문제는, 모든 조합을 구하는 문제이다. 예를들어서 a - 2, b - 2, c - 2가 있다고하면 의상을 1개만 입는 경우, 2개, 3개 입는 경우를 모두 고려해볼 수 있다.
* 1개만 입는 경우의 수는 2 + 2 + 2 = 6이다. 
* 2개만 입는 경우의 수는 2 * 2 + 2 * 2 = 8이다.
* 3개만 입는 경우의 수는 2 * 2 * 2 = 8이다.

* 해당 규칙을 보고, depth == 1부터 depth == hashMap.size()까지 루프문을 돌아 백트래킹을 진행해 답을 구하면 된다는 생각을 하였다, 예를 들어서 depth가 2이면,  (1, 2) (1, 3) (2, 3)을 뽑아서 곱한 다음에 answer에 더하는 방식으로 하면 된다.

## 🙂 새로 알게된 점
* 생각보다 DFS를 자유롭게 쓸 수 있다는 생각을 하게되었다.