Project Title
==============
Billiards Ball Object Detection(YOLOX + ByteTrack + VideoExtraction)

Motivation
===============
I propose a new trained billards ball detector in 'Independent Learning and Research(독립심화학습)' class at KHU.

다양한 분야, 특히 스포츠 산업에서의 인공지능의 적용을 시도하고 싶었습니다. 
많은 기술이 적용되고 있는 골프와 달리 한국 당구는 오픈 데이터가 존재하지 않고, 기술의 실시간 적용이 부진한 상황이었습니다.
특히나 3구, 4구와 같은 당구 스포츠는 초보자에게 진입장벽이 높아 이를 해소할 수 있는 기술을 개발하고자 합니다.

Process
====================
저는 3-stype으로 나눠 Billards Skill Prediction 과제를 수행하고자 합니다.

(1) 당구 공 Object Detetor를 학습시킨다.

(2) 당구 공 궤적 데이터와 (수구, 제1목적구, 제2목적구), kiss 여부, score 여부, 마지막으로 기술을 라벨링한 데이터를 데이터베이스에 저장한다.
    (2)-1 당구 공 궤적 데이터 일부만 기술을 라벨링한 뒤, 예측기를 학습하여 나머지 데이터를 전부 라벨링한다.
    
(3) 정지한 3구 당구공이 주어졌을 때, 제1목적구를 설정한 뒤 K-NN을 사용하여 kiss 여부, score 여부에 따른 비슷한 상황을 추천한다. 




Demo Video
============
1. YOLOX (3구)

![yolox_crop](https://user-images.githubusercontent.com/87460971/174051289-34685a51-e170-477f-85ad-ee132a2f446d.gif)


2. Byte-Track (4구)

![ByteTrack_crop](https://user-images.githubusercontent.com/87460971/174052157-d771ad25-e11d-441f-863e-1d84eddce723.gif)
