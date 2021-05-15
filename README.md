# ML_MNIST-Project

# 머신러닝 지정과제
Fashion MNIST Data를 사용하여 각각의 Object를 classification. <br>
SVM, DecisionTree, RandomForest 모델들을 파라미터 튜닝을 통해 최대 Accuracy를 구한다.

# Data
### Fashion MNIST
<img src='fashion_MNIST_sample.png' width = 500>

#### Train set : 1000 &nbsp;&nbsp;&nbsp;  Test set : 1000

# Model
### SVM

<img src = 'https://user-images.githubusercontent.com/77375223/118351034-8c62bb00-b594-11eb-8202-241b764f34e6.png' width = 500>


Data들간의 집합을 통하여 선형 분류기로 분류 (Kernel Trick으로 비선형 Task에도 적용 가능)<br>

사용한 Kernel : Gaussian Kernel <br>

gamma, C로 모델의 복잡도 조절 가능 <br>

gamma : 1e-3, C : 10 사용

validation : 81% <br>
test accuracy : 82%

<br>

### Decision Tree

<img src ='https://user-images.githubusercontent.com/77375223/118351145-2cb8df80-b595-11eb-9bb1-8752940b43d8.png' width = 500>

특정 기준(질문)에 따라 데이터를 분류 <br>

max_depth, max_leaf_nodes ... 등등 여러개의 규제 매개변수가 존재 <br>

max_depth : 9, max_features : 4, max_leaf_nodes : 37 사용

validation : 64% <br>
test accuracy : 66%
<br>


### RandomForest Tree

<img src = 'https://user-images.githubusercontent.com/77375223/118351202-802b2d80-b595-11eb-94f4-cd8108cfe07c.png' width = 500>

결정트리들을 앙상블 한 것.

앙상블 : Bagging, max_depth : 8, n_estimators : 100

validation : 80% <br>
test accuracy : 81%
