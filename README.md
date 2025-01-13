# 🎯 화살 피하기 게임

모바일 기반으로 제작된 화살 피하기 게임은 간단한 컨트롤과 직관적인 인터페이스를 활용하여 누구나 쉽게 즐길 수 있는 게임입니다. 객체 풀링 및 다양한 유니티 기능을 활용하여 성능을 최적화하였습니다.

---

## 🎥 유튜브 데모 보기

[![유튜브 데모 보기](https://img.youtube.com/vi/RH5r6KlxC9s/0.jpg)](https://www.youtube.com/watch?v=RH5r6KlxC9s)




## 🏹 01. 화살 피하기 - Arrow

### 화살 생성 및 방향 설정
- 화살 방향은 **플레이어를 항상 바라보면서 생성**됩니다.
- **객체 풀링(Object Pooling)**을 통해 객체의 생성과 삭제를 최소화하였습니다.

<img src="https://raw.githubusercontent.com/wanna175/2Dgame/main/img/arrow01.PNG" alt="화살 방향 설정" width="600"/>

---

### 각도 계산
- 화살 스프라이트는 오른쪽 방향 기준으로 설계되었습니다.
- **Vector.right**와 **(플레이어 위치 - 화살 생성 위치)** 백터의 내적값을 통해 각도를 계산합니다.
- 생성 위치보다 플레이어 위치에 따라 화살 객체를 **degree 값에 따라 z축 회전**시켜줍니다.

---

### 객체 풀링
- **화살 객체(Arrow)**는 **큐(Queue)**에 미리 생성되어 게임 중 **생성과 삭제 횟수**를 줄였습니다.

---

## 🎮 02. 화살 피하기 - Joystick

### 가상 방향키 구현
- **모바일 기반**으로 제작되어 사용자가 화면을 터치하면 **누른 위치에 가상 방향키**가 나타나도록 구현하였습니다.
- Unity에서 제공하는 다양한 **이벤트 핸들러 인터페이스**를 상속받아 사용하였습니다.

<img src="https://raw.githubusercontent.com/wanna175/2Dgame/main/img/arrow2.PNG" alt="가상 조이스틱 구현" width="600"/>

---

## ⚙️ 03. 그 외의 기능

### 캐릭터 선택 및 스킬
- 사용자가 원하는 캐릭터를 선택할 수 있도록 구현하였습니다.
- **캐릭터마다 고유 스킬**을 설정하고 스킬에 따라 플레이 스타일을 다르게 하였습니다.

<img src="https://raw.githubusercontent.com/wanna175/2Dgame/main/img/arrow3.PNG" alt="캐릭터선택화면" width="600"/>

---

