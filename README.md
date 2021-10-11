# MiD (Medical Image Deep Learning Framework)


## 1. Instructions

- (Korean)
https://glittery-dawn-b91.notion.site/MiD-6ed046f1b3f74b12bb05e29eed32c7c2
- (English)


## 2. Features

### 1. Fully Vectorized Data Augmentation Methods
![스크린샷 2021-10-12 오전 3 28 58](https://user-images.githubusercontent.com/68293683/136837339-4d2836f1-9ad1-4187-b5b9-8a0e6b7e3c81.png)

![스크린샷 2021-10-12 오전 3 29 15](https://user-images.githubusercontent.com/68293683/136837365-2c2534e8-e668-42c5-a5af-89decb96a970.png)

![스크린샷 2021-10-12 오전 3 29 50](https://user-images.githubusercontent.com/68293683/136837440-15a8d492-75c7-4db8-a149-e37d714d460d.png)


### 2. Optimized Resampling Methods
- Fully Vectorization support, unlike existing medical image frameworks.
- GPU method support for full patch size model.
- Computational speed improvement by more than 50% compared to the previous one.


### 3. Solving Class Imbalanced problem
- Application of nnUNet's oversampling technique.
- Automatically extract the oversample Patch with the default value.
- Support for calculating class weights.


### 4. TensorBoard
- Automatically record loss on the tensorboard when using the trainer.

### 5. Optimized Default Values
- The default of the preprocessing values is set to the default registered in the SOTA.

### 6. Scalability
- Connected to pytorch methods
