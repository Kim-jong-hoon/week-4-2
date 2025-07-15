# CNN에서 ReLU와 Softmax란?

CNN(Convolutional Neural Network, 합성곱 신경망)에서 `ReLU`와 `Softmax`는 **활성화 함수(Activation Function)**로 사용되며, 서로 다른 목적을 수행합니다.

---

## 🔹 1. ReLU (Rectified Linear Unit)

**정의**:  
ReLU는 입력값이 0보다 크면 그대로 출력하고, 0 이하이면 0으로 출력하는 함수입니다.


**특징**:
- **비선형성**을 부여하면서도 계산이 간단함
- **음수 값을 제거**하여 신경망을 더 간단하게 학습
- **기울기 소실 문제(Vanishing Gradient)**를 완화함

**사용 위치**:  
- CNN의 **합성곱층(Convolutional Layer)** 또는 **은닉층(Hidden Layer)** 뒤에 주로 사용


## 🔹 2. Softmax
정의:
Softmax는 여러 클래스 점수를 확률 값으로 정규화하는 함수입니다. 출력값의 총합은 1이 되며, 각각을 확률처럼 해석할 수 있습니다.

Softmax(z_i) = e^(z_i) / Σ e^(z_j)
<br>**특징**:
<br>- 출력값은 0과 1 사이의 실수
<br>- 총합이 1이 되는 확률 분포 생성
<br>- 어떤 클래스에 속할 확률처럼 해석 가능

사용 위치:

CNN의 **출력층(Output Layer)**에서 주로 사용
