Day2
------------------------------------------
1. tensorflow로 간단한 linear regression을 구현
- 파이토치를 활용할거기 때문에 tensorflow는 건너뛰겠다.

2. linear regression의 cost 최소화 알고리즘의 원리 설명
- loss fuc의 최솟값 구하기 gradient descent algorithm
- 기울기가 음수일때 W가 + 쪽으로, 양수일때 W가 -쪽으로
- New Weight = Weight - (learning rate* loss fuc 미분)
- loss fuc 모양확인

3. multi-variable linear regression
- H(x1,x2,x3) = w1*x1 + w2*x2 + w3*x3 + b
  1.maxtrix 표현하기
  - (1x3) (3x1) = XW
  
4. Logistic Classification의 가설 함수 정의
- 0 ~ 1 사이로 함축
- sigmoid function -> G(H(x))
- local minimum 문제 생김
- C:(H(x),y) = -y log(H(x)) - (1-y) log(1-(H(x))
