Day 5
==================================
### 1. neural net for XOR
- weigth의 크기를 잘 맞추어 주어야함
- tensorflow 예제를 통해서 layer 1개와 2개를 비교하여 보여줌
- layer의 중간 출력값을 많이 줘보자 -> 학습이 더 잘된다.
- tensorboard 사용하기
-------------------
### 2. Lecture10 sigmoid 보다 ReLU가 더 좋아
- backpropagation과 sigmoid를 여러층에 걸쳐서 쓰게되면 -> gradient vanishing 문제 발생
- sigmoid 말고 다른함수를 사용 -> ReLU(Rectified Linear Unit) y = max(0, x)
- maxout, ReLU, tanh 등 activation function
-------------------
### 3. weigth 초기화 잘해보자
- 초기값을 0으로 주게 된다면? -> gradient vanishing 문제
- Restricted Boatman Machine(RBM) 
  - 초기 x값과 backpropagation을 통해 돌아온 x값이 최대한 같은 weight
  - encoder라고 부름 -> Fine Tuning 발전
  - 하지만 RBM은 복잡하다. -> 2015년도 Xavier/He initialization
- 아직까지 많은 연구가 이루어지고 있음
-------------------
### 4. Dropout과 앙상블
- overfitting?
  - very high accuracy on the trainning dataset -> poor accuracy on the test data set
  - 깊은층을 쓴다며 발생할 확률이 높음
  - 기본적 해결방법 : 많은 training dataset OR Regularization
- dropout : 랜덤하게 몇몇 node들을 꺼버린다 학습시에만 사용
- ensemble : 여러가지 모델을 써서 합쳐줌 2%정도의 정확도 향상
- 다양한 방법으로 층을 쌓아볼 수 있다. merge, split, current 
