## Info
<a href="https://www.acmicpc.net/problem/1744" rel="nofollow">1744_수_묶기</a>

## ❗ 풀이 방법
1. 해당 수열은 음수와, 0, 양수가 존재하는 수열이다. 두개의 원소를 곱했을 때 가장 큰 값이 나올려면 양수인 경우에는 가장 큰 두수끼리, 음수에서는 가장 작은 두수끼리 곱하면 된다.
2. 그리고 주의해야 될 점은 0과 1이다. 0은 더할 때 아무런 쓸모가 없는 숫자지만, 음수에다가 곱하면 사라지는 특성이 있다. 이를 이용해서 minHeap에 원소가 남았을 때 0을 곱해서 사라지게 하는 역할을 한다.
3. 1은 양수에다가 곱하면 해당 수 그대로 나온다. 따라서 이 수가 나왔을 때는 곱하는 것이 아니라, 더하면 더 큰수를 만들 수 있다.
4. 위에서 말한 로직을 maxHeap과 minHeap을 사용해 문제를 풀면 된다.

## 🙂 새로 알게된 점

* 

