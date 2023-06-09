## Info
<a href="https://www.acmicpc.net/problem/12904" rel="nofollow">12904_A와 B</a>

## ❗ 풀이 방법
- 해당 문제는 케이스별로 손으로 하나씩 구현하면서 규칙을 찾아서 풀면된다.
- 만약에 A → B가 되는 케이스를 dfs로 구할려고 하면 최대 2^1000승이 나와서 매우 비효율적으로 구하게 된다. 그리고 시간도 초과된다.
- 즉, BAA는 무조건 B에 속하고, AAB는 무조건 A에 속한다. 무조건 A아니면 B에 속하는 구조이다.
- 그리고 보면 A또는 B로 끝나는 것을 볼 수 있다. 이걸 이용해서 제일 끝의 인덱스가 A면 A를 제거하고, B면 B를 제거하고 reverse하면 된다.
- 이를 반복해 S의 길이와 같거나 클때까지 반복하고, T가 S가 되면 1, 아니면 0을 반환한다.

## 🙂 새로 알게된 점

* 

