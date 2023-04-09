# Driver-FaceRecognition

### 연구 목표
- Face detection을 위한 얼굴의 특징과 위치 출력  
- kNN알고리즘을 이용하여 Face identification 구현  
- 면허증 주인과 실제 운전자가 동일인인지 식별  
------
### 연구 방법
<img width="60%" src="https://user-images.githubusercontent.com/108534619/230791427-2fafd8fe-9898-4d47-85e9-f51cbb83ff90.png"/>  
<img width="60%" src="https://user-images.githubusercontent.com/108534619/230791488-2f540c1a-f8a4-491d-a40d-2bfe5ddb21c2.png"/>    
<img width="60%" src="https://user-images.githubusercontent.com/108534619/230791494-6d629de3-31bc-4a59-8584-c1a535be649b.png"/>  

----
### 연구 결과
1. 아이돌 식별 결과  
<img width="60%" src="https://user-images.githubusercontent.com/108534619/230791491-5d432517-8d74-4ea2-aea0-a5ad6f1b0d58.png"/>    

2. 운전자 식별 결과  
<img width="60%" src="https://user-images.githubusercontent.com/108534619/230791492-63f3957d-1c0a-445b-ab0f-3464fcb19089.png"/>    

- 동일인 식별을 위한 kNN 알고리즘 구현
- 학습이 굉장히 빠르게 진행됨(idol(100명) training시 6m 24s, 운전자 training시 3s)  
- 아이돌 100명을 한번에 training 했을 때 정확도가 0.91로 높았으며 거의 모든 사람을 올바르게 예측함  
- 아이돌 dataset을 각 그룹별로 나누어서 training 했을 때는 모든사람을 올바르게 예측함  
- 식별하고자 하는 운전자 사진을 training했을 때 해당 사람이 test이미지에 한 명으로 인식되고, 운전석(이미지의 오른쪽)에 위치한다면 운전자가 맞다고 출력됨  
- 정보가 없는 얼굴은 unknown으로 예측
