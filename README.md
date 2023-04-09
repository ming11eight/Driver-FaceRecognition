# Driver-FaceRecognition

- 동일인 식별을 위한 kNN 알고리즘 구현
- 학습이 굉장히 빠르게 진행됨(idol(100명) training시 6m 24s, 운전자 training시 3s)  
- 아이돌 100명을 한번에 training 했을 때 정확도가 0.91로 높았으며 거의 모든 사람을 올바르게 예측함  
- 아이돌 dataset을 각 그룹별로 나누어서 training 했을 때는 모든사람을 올바르게 예측함  
- 식별하고자 하는 운전자 사진을 training했을 때 해당 사람이 test이미지에 한 명으로 인식되고, 운전석(이미지의 오른쪽)에 위치한다면 운전자가 맞다고 출력됨  
- 정보가 없는 얼굴은 unknown으로 예측
