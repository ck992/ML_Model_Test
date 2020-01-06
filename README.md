# Title / Machine Learning Model Test (업로드예정)
* Classification Classification Classification of Credit Approval Data Set by UCI Machine Learning Lab
* UCI data repository 중에서 credit approval data set을 선택하여 credit 유무의 이진 분류로 결정하는 문제를 기계학습모델을 이용하여 해결한다.

Credit Approval Dataset:
*  http://archive.ics.uci.edu/ml/datasets/Credit+Approval

## Installation
* Python 3.x 버젼으로 구축되어있습니다.
* Anaconda 와 Spyder 환경에서 작동하였습니다.
* 코드상 패키지를 pip명령어를 사용해 설치하여 주십시오.

## Process
* step1: Canonical Models의 Decision Tree와 Multilayer perceptron을 평가
* step2: Committee Machines의 Random Forest를 평가
* step3: Deep learning Model의 CNN모델을 평가
* step4: 학습모델의 학습 및 평가는 10-fold 평가방법을 사용한다; 즉, 전체 자료를 10등분한 후에 9 등분을 학습에 나머지 한 등분을 평가에 사용한다. 그리고 이
과정을 10번 반복한 후에 평균을 내어 각 학습모델을 평가한다
## Data Type
A1 부터 A16까지의 attribute가 존재하며 연속형 데이터와 비 연속형데이터가 존재한다. 또한 “?”의 결측 값 역시 존재한다. 또한 이진분류를 위한 target data는 +,-형태로 A16에 나타나 있다.
![uci](https://user-images.githubusercontent.com/26376653/71790545-5cd4a200-3074-11ea-8710-a2f2ffe1e130.png)
## Data Preprocessing
“Credit approval dataset”의 attribute는 총 16개로 이루어져 있으며 연속 및 불연속데이터가 혼합 되어있다. 기계학습 모델에 적용시키기 위해선 그림2 의 dataframe을 모델에 맞게 데이터 전처리 과정을 해야한다. 데이터 전처리과정은 먼저 dataframe형태로 진행되었으며, “?”로 표기된 결측치를 제거시켜 주었다. 또한 A2, A3, A8, A11, A14, A15의 연속형 데이터를 float형태로 데이터 타입을 변경하여 주었다. 속성과 클래스를 다음과 같이 분리시켜 준다. 이진 분류를 결정하는 문제이므로 A16에 존재하는 +,- 데이터를 target으로 선정한 후 0과 1의 형태로 변환 시켜 준다. 또한 학습 및 예측에 사용될 데이터를 나눠 주었다. 

## Step2: Cononcial Model (Decision Tree & Mulitilayer perceptron)
### Decision tree
 Binary classification을 하기 위해, 먼저 정규 모델의 Decision Tree 모델을 사용했다 Decision Tree의 깊이는 3으로 설정하였으며, 모델의 Overfitting을 방지하였다. 그리고 엔트로피를 불순도 계산 방법으로 적용하여 모델을 학습시켰다.
## Step3: Committe Machine (Random Forest)
## Step4: Deep Learning Model (CNN)
## Step5: 학습모델 평가
## Step6: 결론

## Limitations
Cononcal model과 Committee machine의 경우 Scikit-learn의 패키지 사용함. Multilayer perceptron의 경우 정확도(accuracy)가 0.6내외로 평가됨.

## Contact
작동에 문제가 생기시거나 궁금한점이 있으시면 연락주시면 감사하겠습니다 [https://ck992.github.io/](https://ck992.github.io/).
