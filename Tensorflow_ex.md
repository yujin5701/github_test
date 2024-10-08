딥러닝 개요
---
1. 모델을 정의한다: 어떤 식으로 모델을 구성해서, 모델의 정답률을 어떤 지표를 통해 측정할 것이며, 정답률을 높이기 위한 방법은 어떤 식으로 정의할 것인다. 이런 전체적인 디자인을 하는 것.
2. 선형회귀와 GD
- ex) 운동 시간이 늘어나면 체중 감소량도 커진다(선형,Linear 증가. 비례, 반비례 등)
- 앞으로 등장할 새로운 데이터도 한 직선이 추세를 크게 벗어나지 않을 것이라는 합리적인 추측!
- h(x)=wx+b 이라는 가설의 가중치(기울기)와 편향(y절편)을 찾아내는 것이 핵심!
  Cost Function
- 컴퓨터는 선형을 수치화해서 계산해야 함. 즉, 가설 h(x)와 실제값(y)의 차이를 오차라고 하고, 이 오차가 최소화 되는 w와 b를 찾아야 함.
- 전문 용어: 목적함수, 비용함수, 오차함수 등
- 선형회귀에서의 목적함수 = 최소 제곱 오차: 실제값(h)+예측값(h(x))을 제곱하여 모두 더한 형태.

최적화(목적함수의 값을 최소화 할 수 있게 만드는 작업=최적화 알고리즘)
- cost = aw^2 + bw + c
- 경사하강법(Gradient Decent) 알고리즘
- 머신러닝 알고리즘은 가설을 세우고, 실제 데이터와 예측값을 비교하며 적절한 오차함수를 설정한 다음, 이를 최소화할 수 있는 최적화 과정을 거쳐 모델을 만들어 낸다.

3. 이진 분류, 로지스틱 회귀와 cross entropy: 로지스틱 회귀는 사실 분류 문제를 풀 때 사용
4. 시그모이드(sigmoid) 함수
(1) 이진 분류, 시험 점수에 따른 합/불여부 판별: 선형 회귀와 달리 1차방정식으로 표현하기 힘들다. 직선보다 곡선으로 표현 게 나음
(2) 예를 들어서 55점 이하는 탈락아고, 그 이상은 합격일 때, 이걸 직선으로는 표현하기 좋지 않다. 직관적으로 합격 여부를 확률로 표현할 수 있음
(3) h(z) = 1/1+e^(-z), where z = wx + b
----------
3:10
