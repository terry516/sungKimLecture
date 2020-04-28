Day 6
===========================
### 1. Lecture11 convNet의 conv layer 만들기
- 고양이의 뇌를 보고 제작
- 사진을 잘라서 부분부분을 layer에 input 크기는 (32x32x3)
- Output size = (N-F) / stride + 1 , 너무작아지는 것을 방지하기 위해 padding
- activation maps의 depth는 filter의 개수
- filter의 weight를 학습시켜나간다  
### 2. Max pooling 과 FC
- pooling -> resizing , parameter 수가 너무 많아져서 overfitting을 방지하기 위해서
- FC layer -> 앞에서 본 일반적인 layer  
### 3. CNN case study
- LeNet, Alex Net, google Net
- ResNet -> 152 layer로 층이 매우 많지만 H(x) = F(x) + x 로 짧게 만드는 느낌을 줌
- text를 conv Net으로 처리해 보자
- 앙상블 해보기
