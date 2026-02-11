아직 정규화된 교육과정이 없다. IBM 계정 만들기
크레딧은 한달정도 쓸 수 있다(!)

2/9
whats a quantum superposition
양자 역학을 가지고 컴퓨터가 작동함.
중첩현상 설명 - 고전역학에서는 이걸 설명할 수가 없음. 위 또는 아래로만 가야하는데, 중첩이 발생함.
중첩은 노이즈캔슬링같은데서 우리가 이미 뭔지는 아는 것임.

실험적 증거가 많다.
Stern Gerlach experiment
Bell's inequality - 고전역학을 가정할 시 최대가 2인데 양자역학에서는 2루트2를 얻을 수 있다.
실험적으로 이것이 추후에 증명된다. 이해하기 힘들 순 있지만 작동한다.

Hadamard - 축변환, Sgate, Tgate는 각도 돌리기,
CNOT은 두개의 양자상태가 얽히게 만들 수 있음. 이게 노이즈 제어등이 워낙 어려워서 성능을 결정함.
양자 회로도 만들어볼거임! 처음엔 0에서 시작함.
Hgate가 Y축 로테이션이었다면, Sgate는 Z축 기준 회전, pi/2만큼 회전. Tgate는 Z축 기준인데, pi/4만큼만 돌린다.
에러코렉션이라는 게 가능한데서는 이 T게이트가 어렵다.

실제 양자 알고리즘을 만드는 것은, (IBM Quantum Experience). .게이트를 배치하는 것.

Shor's Algorithm을 보겠다.
RSA에 대한 기초 설명, 이게 어디에 쓰일 수 있느냐 라는 그런 논의.
Harvest Now, Decrypt later라는 개념.

게이트 자체가 오류를 내기에 보통 오류율 0.1%를 가정.
physical qubit 여러개를 묶어 공고한 logical qubit을 만든다.

그다음 여기 bits-gates-and-circuits 가지고 회로 짜가지고 테스트하고 있다.

//오후세션
양자머신러닝
행렬을 대각화할때 양자컴퓨터를 쓸 수 있다!

고전머신러닝은 샘플을 가지고 학습하는데, 양자머신러닝은 샘플의 양자중첩을, 병렬성을 가지고 빠른학습을함.

NISQ 시대가 도래 -> 오류, 중규모, 실현가능한 양자.

양자이득의 구현 및 적용
단기활용가능성에 대한 비젼, 응용사례 발굴의 시대이다.

Early FTQC로 넘어가는 중.

참고- 시뮬레이션하면 그냥 다 보는 거임. 관측을 할 필요가 없음.

///
2/10 허준석

QPE 를 볼건데, 푸리에변환을 알면 좋다.
Time Series 에서 Eigenvalue를 추출하려면 Hamiltonian, 푸리에 변환을 거쳐야한다.

Resolution은 현실에선 finite하기에, 한계가 생긴다. (??)

Time <> Frequency and uncertainty
시간에 따라 여러가지 EigenValue들이 섞인다. 이를 양자를 통해 해결하고자 한다.

양자에서 중요한 문제는 open problem - E10을 알려면 c10이 존재해야하고, 이에 맞는 initial state를 정의할 필요가 있다.
e-ieKt 는 시간에서 델타function

양자로 하는거랑 고전역학적으로 찾아내는 것이랑,
힐버스 스페이스 증가, resolution 증가, 푸리에 변환에 의한 분석.
//
오후 박경덕

고전컴퓨터랑 하이브리드가 협업하는게, Krylov Subspace Diagonaliztion에서 양자컴퓨터가 subspace를 선택하면 그 안에서는 다시 고전컴퓨터 이용.

오후 백경현
grover's algorithm.
grover 에서는 Oracle, Reflction이 한 액션.

t-depth-optimized quantum search with quantum data-access machine.

//
2/11
VQE,VQA optimization 등으로, 기본 개념 정립.
양자시뮬레이션 - 파인만.
Richard Feynman put it in memorable words: “Nature isn't classical, dammit, and if you want to make a simulation of nature, you'd better make it quantum mechanical, and by golly it's a wonderful problem, because it doesn't look so easy.”

수소만해도 analytical하게 풀 수 있는데, 헬륨, 2개만해도 디럽게 어려워져서 못한다!
물분자나, 단백질 등 복잡한 걸 풀어야 의미이는 일을 할 수가 있을텐데.

1982년 파인만이 양자컴퓨터를 제안.

양자 컴퓨터가 양자 시뮬레이션을 할 수 있는 이유다. Trotterization을 어떻게 풀 것이냐의 문제.
N개가 있을 때 고전컴은 2^n을 하는건데, 양자컴퓨터는 n개 큐빗으로 처리?

QAOA
https://www.nature.com/articles/s41534-021-00368-4
//오후. 박미리 - IBM <> 연대 POC
Hamiltonian Simulation 영역에서 우월성 증명이 우선과제다.
QML, PDE solving도 계획중.
//한남식
High Attrition rate. 임상1차, 2016년 기준 전체 10%도 안되고, 암은 5% 정도.
제 예측은, 퀀텀 역시 인공지능과 비슷한 길을 갈 것.
30년이면 양자가 꽤 커질 것이다.

Network Analysis - Random walk을 통해서, 각 단백질마다 점수를 주게 된다. Alan turing이 고안.
Quantum walk은 Random walk과 관련이 있다.
네트워크상에서 워커가 다음 방향을 정할 때, 하나를 정하는 게 아니라 중첩을 시켜 동시에 여러가지로 걸어보자~
