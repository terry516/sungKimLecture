Day 7
==============================
### 1. Lecture12 NN의 꽃 RNN 이야기
- sequence data를 어떻게 처리할까?? (음성인식, 글)
- recurrent neural network ( new state = f(old state, x) ) , function은 모두 같음
- 가장 기본적인 RNN (vanilla) h = tanh(w1*h + w2*x), y = w3 * h
- recurrent한 layer의 function이 모두 같음 -> w1, w2, w3를 모두 같이 쓰는것임
- 초기 h값은 없기 때문에 초기값으로 0 놓을때가 많다
- language modeling, speech recognition, machine translation, image/video captioning 등
----------------------------------
이후 동영상들은 tensorflow 실습 동영상으로 참고
