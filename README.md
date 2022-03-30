# computervsion_classification
classification 모델을 다양한 모델, 방식을 적용하여 구현합니다.

# 1.Resnet  [[GitHub link]](https://github.com/minigoom/computervsion_classification/blob/main/Resnet%20model.ipynb)
- Resnet 34, Resnet 50 모델 구현
- plain 34, plain 50 모델 구현
- tensorflow dataset cat vs dog data를 이용하여 성능을 평가해봄
- accuracy 측면으로 Resnet 34, Resnet 50, plain 34, plain 50 모델순으로 낮게 측정되었다.
- ![image](https://user-images.githubusercontent.com/97006756/159713492-2aa62954-45c0-4111-92cb-dae232dd6bb3.png)

# 2 mnist classification [[GitHub link]](https://github.com/minigoom/computervsion_classification/blob/main/mnist_classification.ipynb)
- dataset 
  - 0 ~ 9 까지 손글씨 데이터로 구성
  - size : 28 x 28
  - 60,000 train data, 10,000 test data
- cnn 활용하여 모델 구현
  - 하이퍼파라미터 수정전: 0.9899
  - 하이퍼파리미터 수정후: 0.9901
- 모든면에서 하이퍼파라미터 수정후(after)가 수정전(before) 보다 뛰어나다.
<img src="https://user-images.githubusercontent.com/97006756/159900197-e041cd66-c2de-419e-a7cb-dd3b84cd4475.png" width="400" height="300"/>

# 3 VGG [[GitHub link]](https://github.com/minigoom/computervsion_classification/blob/main/VGG_model.ipynb)
- dataset
  - cifar10
  - size : 32x32x3
- VGG16, VGG19 모델 구현
  - 모델 block 을 생성하는 함수 구현
  - 모델을 생성하는 함수 구현
- 모델이 전제척으로 VGG16이 VGG19보다 좋게 측정되었다.

# 4 apply Augmentation, cutmix, mixup to resnet50 model  [[GitHub link]](https://github.com/minigoom/computervsion_classification/blob/main/augmentation%2Ccutmix%2C%20mixup%20with%20resnet50.ipynb)
- dataset
  - standford dog
- augmentation 적용
  - random_flip_right
  - random_brightness 
- cutmix 적용
- mixup 적용
- mixup, cutmix 를 epoch= 20으로 학습하였을때 accuracy가 더 낮게 학습되었다. 그래서 학습을 더 시키면 성능이 좋아지지 않을까? 라는 생각을 하였고 epoch = 50 으로 학습시켰다. 하지만 별로 차이가 있는 결과를 얻지 못하였다.[[Github link]](https://github.com/minigoom/computervsion_classification/blob/main/agumentation%2C%20cutmix%2C%20mixup%20with%20resnet50(epoch%2050).ipynb)
