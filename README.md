---
CBNU: Huro
---
## HW
+ WAVEGO `12-DOF Bionic Dog-Like Robot`
  + 12개의 자유도를 갖는 4족 보행 로봇 : [WAVEGO wiki](https://www.waveshare.com/wiki/WAVEGO)

## SW
+ Sublime
+ Arduino IDE

## Languages
+ C/C++/html
+ Python3

## Arduino : ESP 32
Demo코드에서 추가적인 행동함수 추가로 정의
- 앉기
- 일어나기
- 오른손 악수
- 왼손 악수
- 손 내밀기
- 손 내리고 원위치
- 엎드리기
- 일어나기

## Raspberry Pi 4B
- opencv를 활용해 사람을 detecting하고 고개(카메라)가 객체를 따라가는 기능 추가 (findColor 기능 수정 => 움직이는 사물 탐지하고 움직이며 추적함)
  - openCV로 객체 마스킹하고 마스크가 일정 좌표 벗어나면 로봇 앞 서보모터들의 움직임을 통해 카메라 센서가 추적할 수 있도록 기능 개선
- 파이썬으로 pyserial 라이브러리를 통해 시리얼 통신을 설정하고 정의한 움직임들을 호출하여 사용

- 이미지 전처리 → 배경 모델 → 프레임 간 차이 계산 → 윤곽 처리 → 움직임 감지

---
### 아쉬운 점
- OPENCV를 이용한 영상 처리만 활용하고 AI 모델 기반으로 정확한 객체 인식 기능을 구현 X
- 통신이 원활하게 되지 않아서 오작동 -> 당시 배터리 출력 부족으로 원인 판단

![ㅋㅋㅋㅋ](https://github.com/6eom9eun/cbnu_huro/assets/104510730/597e834b-c90a-4b37-8f1f-88e3283bef7f)
