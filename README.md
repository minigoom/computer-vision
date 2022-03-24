# computervsion_classification
classification 모델을 구현합니다.

## 1.Resnet  [[link]](https://github.com/minigoom/computervsion_classification/blob/main/Resnet%20model.ipynb)
- Resnet 34, Resnet 50 모델 구현
- plain 34, plain 50 모델 구현
- tensorflow dataset cat vs dog data를 이용하여 성능을 평가해봄
- accuracy 측면으로 Resnet 34, Resnet 50, plain 34, plain 50 모델순으로 낮게 측정되었다.
![image](https://user-images.githubusercontent.com/97006756/159713492-2aa62954-45c0-4111-92cb-dae232dd6bb3.png)

# 2 mnist classification [[link]](https://github.com/minigoom/computervsion_classification/blob/main/mnist_classification.ipynb)
- dataset 
  - 0 ~ 9 까지 손글씨 데이터로 구성
  - size : 28 x 28
  - 60,000 train data, 10,000 test data
- cnn 활용하여 모델 구현
  - 하이퍼파라미터 수정전: 0.9899
  - 하이퍼파리미터 수정후: 0.9901
- 모든면에서 하이퍼파라미터 수정후(after)가 수정전(before) 보다 뛰어나다.
![image](https://user-images.githubusercontent.com/97006756/159900197-e041cd66-c2de-419e-a7cb-dd3b84cd4475.png)
