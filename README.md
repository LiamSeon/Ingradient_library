# MiD (Medical Image Deep Learning Framework)


## 사용 방법

https://glittery-dawn-b91.notion.site/MiD-6ed046f1b3f74b12bb05e29eed32c7c2


## 특징

### 1. 빠른 Data Augmentation
![스크린샷 2021-10-12 오전 3 28 58](https://user-images.githubusercontent.com/68293683/136837339-4d2836f1-9ad1-4187-b5b9-8a0e6b7e3c81.png)

![스크린샷 2021-10-12 오전 3 29 15](https://user-images.githubusercontent.com/68293683/136837365-2c2534e8-e668-42c5-a5af-89decb96a970.png)

![스크린샷 2021-10-12 오전 3 29 50](https://user-images.githubusercontent.com/68293683/136837440-15a8d492-75c7-4db8-a149-e37d714d460d.png)



(Custom이 MiD를 뜻함.)

### 2. 최적화된 Resampling
- 기존 medical image framework들과 달리 완전한 Vectorization 지원.
- Full Patch Size 모델을 진행할 때는 GPU 메소드 지원
- 기존 대비 50% 이상 속도 향상.


### 3. Class Imbalance 해결 파이프라인 구축
- nnUNet의 Oversampling 기법 적용.
- Default 값으로 자동으로 Oversample Patch를 뽑아냄.
- Pipeline상에 Class Weight 적용 지원


### 4. TensorBoard 지원
- trainer 사용 시 자동으로 tensorboard에 Loss 기록

### 5. 최적화 파이프라인
- 전처리 값들의 Default가 SOTA에 등재된 Default로 맞춰져 있음.
- 모든 메소드들에 대한 Vectorization 진행.

### 6. 확장성
- 모든 Pytorch Module과 확장 가능
