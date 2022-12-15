
AI+x: Deep learning Project
-
    Merry X-Mas :)
    Dec.13


video: ""
<img width="1000" src="https://user-images.githubusercontent.com/117716335/207118416-177fd306-a708-4779-ac1c-f53d3c0d5ef3.png"/>

# computer-vision---classcification-of-bottles


abstract : 

팀원
-
> 
유동석_Erica_응용물리학과_2020016626, boo417@hanyang.ac.kr 

목차
-
- Introduction
- Dataset
- Method
- 4

Introduction
-

-01
재생 플라스틱 섬유

재활용 쓰레기 플라스틱 그리고 바다,산 등 다양한 곳에서 발견되는 플라스틱쓰레기들을 재생 플라스틱 섬유라는 옷, 신발 등에서

사용되는 재료로 특별한 공정을 통해서 바꾸게 된다.

<img width="1000" src ="https://user-images.githubusercontent.com/117716335/207230693-49ec9759-d809-43c8-bba9-b46d98e20575.png"/>


팔리 오션 플라스틱(Parley Ocean Plastic™) 와 아디다스는 2017년 

해양 플라스틱 쓰레기를 통해 운동화 제작 협업을 하기도 하면서, 이와같이 플라스틱 쓰레기 재활용의 특별함을 보여주고 있다


- # 02 : 재생 플라스틱 섬유 공정 중 어려움

이런 재생 플라스틱 섬유로 바꾸는 공정 중 어려움을 겪고 있다. 바로

" 플라스틱의 색깔에 맞게 플라스틱들을 골라내야하는데 사람이 직접 골라내야한다는 것"
--
플라스틱 재생 섬유를 만드는데 있어서 색깔 별로 플라스틱을 골라내고, 골라진 플라스틱을 잘게 부숴 전처리 과정이 있다.

따라서 인력이 쓰이게 되며, 상당히 반복적이고 고된 작업이다.

이를 해결하기 위해서 카메라와 인공지능으로 이런 작업을 대체하려고 한다.

이번 시간에서는 우선 문제 해결을 위해 mask R cnn 을 이용한 각 색깔별로 플라스틱 인식을

구현해보려고 한다. 따라서 직접 현장에서의 문제 상황을 가정한다.

https://youtu.be/1rGSle4hICs

현재 갈색 플라스틱 병들 중 흰색 플라스틱 병들을 골라내야하는 상황


문제 해결 : 갈색 , 흰색 플라스틱 병들을 인식하기


사용 할 것 : Mask R cnn , 이미지 라벨링 사이트



Dataset
-


우선 유튜브에 공정 과정을 녹화하여 train(20개), validation(5개) 이미지 데이터를 준비한다.


Method
-

- Mask R cnn  


Mask R cnn = Fast R cnn + Faster R cnn + Fully Convolution Network
