## P=NP? P≠NP?
P 대 NP 문제에 대한 정확한 설명은 Stephen Cook 이 그의 선구적 논문 **"The Complexity of Theorem‑Proving Procedures"** (1971) 과 같은 시기에 러시아 학자인 Leonid Levin 논문으로 부터 출발했다. Cook-Levin 정리 발표 이후 Richard Karp가 **"Reducibility Among Combinatorial Problems"** (1972) 논문을 통해 21가지 문제가 NP-완전임을 증명하였다.

P=NP는 모든 NP 문제를 P 문제처럼 다항 시간 안에 해결할 수 있는지를 묻는 문제이다. 클래스 P는 결정론적 튜링 기계로 다항 시간 안에 해를 찾을 수 있는 문제들의 집합이고, NP는 해답이 주어졌을 때 그 해를 다항 시간 안에 검증할 수 있는 문제들의 집합이다. 따라서 P ⊆ NP는 자명하다. NP에 속하는 모든 문제는 결정론적 튜링 기계를 사용하여 **부울 만족 가능성 문제(SAT)**로 다항 시간 안에 환원될 수 있다. NP-완전 문제는 NP에 속하며, 동시에 NP의 모든 문제로부터 다항 시간 환원이 가능한 문제를 말한다. 따라서 하나의 NP-완전 문제에 대해 다항 시간 해법이 존재한다면, NP의 모든 문제를 다항 시간에 해결할 수 있으며, 이는 곧 P = NP 임을 의미한다.
<br>
<br>
## NP-완전
### 3-SAT
3-충족 가능성 문제(3-SAT, Boolean satisfiability problem)는 NP-완전의 대표주자이고 모든 문제 환원의 기준이다. 이 문제는 참 또는 거짓의 진리 값을 가질 수 있는 3개의 문자 또는 변수 p,q,r 이 있다. 그리고 논리합으로 연결된 절 몇 개가 논리곱으로 구성된 부울 수식 f가 참이 되도록 문자의 진리 값을 구할 수 있는가를 묻는다.
### Subset Sum / Knapsack
NP완전에서 아주 직관적인 문제중 하나다. 집합의 부분집합 중에서 그 합이 0인 경우가 존재하면 참이 된다 {-1, 3, -2, 4} -1+3-2=0 이 집합은 참이다. 부분집합의 합이 0이 아니라 특정 수로 정하면 Knapsack 문제가 된다.
### Hamiltonian Path / Cycle
Hamiltonian Path: 그래프의 모든 정점을 한번씩 방문하는 알고리즘
<br>
Hamiltonian Cycle: 시작점과 끝점이 동일한 헤밀턴 경로
<br>
### Graph Coloring
그래프의 각 정점에 같은 색깔이 인접하지 않게 칠하는 방법이다. 이것으로 그래프의 불변성을 정의할 수 있다.
### Vertex Cover / Independent Set / Clique
Vertex Cover: 선택한 정점들이 모든 정점들과 연결되어있다. 독립셋과 동치이다. NP의 다항시간 해답 검증이 직관적이다.
<br>
Independent Set: 정점이 서로 연결되지 않는 그래프
<br>
Clique: 부분그래프이면서 임의의 두노드가 서로 연결되어있는 것으로 정의된다. 독립셋과 동치이다.
<br>
### Partition Problem
Subset Sum 의 약식버전

### Set Cover ↔ Hitting Set
Set Cover: 원소들의 집합 U와 부분 집합들의 모임 S가 주어졌을 때, 합집합이 U와 같은 S의 가장 작은 부분 집합을 구하는 문제. 모든 미완성 퍼즐을 완성하기 위해 가장 적은 수의 퍼즐을 찾아야 하는 것.
<br>
Hitting Set: 원소들의 집합 U와 부분 집합들의 모임 S가 주어졌을 때, S의 모든 부분 집합과 교차하는 U의 가장 작은 부분 집합을 찾는 문제. 모든 미완성 퍼즐을 완성하는 데 사용할 수 있는 퍼즐 조각의 가장 적은 개수를 찾아야 한다. 
<br>
설정된 커버 솔루션이 있는 경우, 선택한 세트 내의 요소만 취하면 쉽게 타격 세트를 식별할 수 있다. 반대로, 타격 세트가 있는 경우 타격 세트에서 하나 이상의 요소를 포함하는 모든 세트를 선택하여 세트 커버를 구성할 수 있다.  이 두 문제는 단지 원소와 집합을 덮거나 맞추는 것에 대한 같은 질문을 묻는 다른 방식일 뿐이다. 
<br>
<br>
<br>
<a href="http://pvsnpkr.github.io/LOGIC" target="_blank">논리학</a>
<br>
<br>
<br>
<p align="center"><a href="mailto:provepnp@gmail.com">provepnp@gmail.com</a></p>
