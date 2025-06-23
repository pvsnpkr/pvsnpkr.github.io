## 개요
P 대 NP 문제에 대한 정확한 설명은 Stephen Cook 이 그의 선구적 논문 **"The Complexity of Theorem‑Proving Procedures"** (1971) 과 같은 시기에 러시아 학자인 Leonid Levin 논문으로 부터 출발했다. 결정론적 문제 P는 답을 찾는데 다항시간이 걸리는 문제이고 비결정론적 NP는 답이 주어지면 다항시간내 확인할 수 있는 문제이다. NP에 속하는 모든 문제는 결정론적 튜링 기계를 사용하여 다항 시간 내에 부울 만족 가능성 문제로 환원 될 수 있다. Cook-Levin 정리 발표 이후 Richard Karp가 **"Reducibility Among Combinatorial Problems"** (1972) 논문을 통해 21가지 문제가 NP-완전임을 증명하였다.

P=NP는 NP문제를 P문제처럼 해결할 수 있는가의 문제이다. P가 NP에 속하는 건 자명하다. NP-완전은 NP중에서 어려운 문제로 어떤 NP-완전 문제는 다른 NP-완전 문제로 환원 가능하다. 따라서 NP-완전 문제중 한가지만 해결해도 모든 NP-완전이 해결되며 P=NP 임이 증명된다.
<br>
<br>
## NP-완전
### 3-SAT
3-충족 가능성 문제(3-SAT, Boolean satisfiability problem)는 NP-완전의 대표주자이고 모든 문제 환원의 기준이다. 이 문제는 참 또는 거짓의 진리 값을 가질 수 있는 3개의 문자 또는 변수 p,q,r 이 있다. 그리고 논리합으로 연결된 절 몇 개가 논리곱으로 구성된 부울 수식 f가 참이 되도록 문자의 진리 값을 구할 수 있는가를 묻는다.
### Subset Sum / Knapsack
NP완전에서 아주 직관적인 문제중 하나다. 집합의 부분집합 중에서 그 합이 0인 경우가 존재하면 참이 된다 {-1, 3, -2, 4} -1+3-2=0 이 집합은 참이다. 부분집합의 합이 0이 아니라 특정 수로 정하면 Knapsack 문제가 된다.
### Hamiltonian Path / Cycle
Hamiltonian Path: 그래프의 모든 정점을 한번씩 방문하는 알고리즘<br>
Hamiltonian Cycle: 시작점과 끝점이 동일한 헤밀턴 경로<br>
### Graph Coloring
그래프의 각 정점에 같은 색깔이 인접하지 않게 칠하는 방법이다. 이것으로 그래프의 불변성을 정의할 수 있다.
### Vertex Cover / Independent Set / Clique
Vertex Cover: 선택한 정점들이 모든 정점들과 연결되어있다. 독립셋과 동치이다. np의 다항시간 해답 검증이 직관적이다.<br>
Independent Set: 정점이 서로 연결되지 않는 그래프<br>
Clique: 부분그래프이면서 임의의 두노드가 서로 연결되어있는 것으로 정의된다. 독립셋과 동치이다.<br>
### Partition Problem
Subset Sum 의 약식버전
<br>
<br>
<a href="http://pvsnpkr.github.io/LOGIC" target="_blank">논리학</a>
<br>
<br>
<br>
<p align="center"><a href="mailto:provepnp@gmail.com">provepnp@gmail.com</a></p>
