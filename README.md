# P=NP? P≠NP?
## 개요
P 대 NP 문제에 대한 정확한 설명은 Stephen Cook 이 그의 선구적 논문 **"The Complexity of Theorem‑Proving Procedures"** (1971) 과 같은 시기에 러시아 학자인 Leonid Levin 논문으로 부터 출발했다. 간략히 요약하면 결정론적 문제 P는 답을 찾는데 다항시간이 걸리는 문제이고 비결정론적 NP는 답이 주어지면 다항시간내 확인할 수 있는 문제이다. NP에 속하는 모든 문제는 결정론적 튜링 기계를 사용하여 다항 시간 내에 부울 만족 가능성 문제로 환원 될 수 있다. Cook의 SAT 관련 정리 발표 이후 Richard Karp가 **"Reducibility Among Combinatorial Problems"** (1972) 통해 21가지 문제가 NP-완전임을 증명하였다.
<br>
<br>
<p align="center"><img src="P_np_np-complete_np-hard.svg.png" width="400"/></p>
<p align="center"><b>복잡도 다이어그램</b></p>
<br>
P가 NP에 속하는 건 자명하다. NP문제에 환원은 중요한 개념으로 모든 NP-완전은 SAT으로 환원된다(Cook-Levin 정리). NP-완전 문제중 한가지만 해결해도 모든 NP-완전이 해결되며 P=NP 임이 증명된다.

## NP-완전
### 3-SAT
3-충족 가능성 문제(3-SAT, Boolean satisfiability problem)는 NP-완전의 대표주자이고 모든 문제 환원의 기준이다. 이는 참 또는 거짓의 진리 값을 가질 수 있는 3개의 문자 또는 변수 p,q,r 이 있다. 그리고 논리합으로 연결된 절(clause, c) 몇 개가 논리곱으로 구성된 부울 수식 f가 참이 되도록 문자 의 진리 값을 구할 수 있는가의 문제이다. 즉, 수식 f 가 충족 가능이란 수식 f가 참이 되기 위해 모든 절이 참이 되도록 문자의 진리 값을 얻어야 하며, 모든 가능한 참인 경우 중 한 가지 이상만 얻으면 된다. 반면에, 가능한 모든 문자의 진리 값에 대해 수식 f가 참이 되지 못하면 즉, 수식이 성립하지 않으면 충복 불가능이라 한다.
### Subset Sum / Knapsack
### Hamiltonian Path / Cycle
### Graph Coloring
### Vertex Cover / Independent Set / Clique
### Partition Problem
Subset Sum 의 약식버전
<br>
<br>
# P = NP 라면?
<br>
<br>
<br>
<a href="http://pvsnpkr.github.io/LOGIC">LOGIC</a>

<p align="center"><a href="mailto:provepnp@gmail.com">provepnp@gmail.com</a></p>
