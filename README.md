# Parasite(가제)

본 프로젝트는 개발팀 2인, 아트팀 2인 총 4인으로 진행되었으며, 팀장을 맡아 전체적인 프로젝트 관리를 겸한 본인의 개발 영역은

- 플레이어 입력 및 애니메이션 처리
- JSON 형식 데이터 테이블 구축
- 물리 처리
- 전투 시스템 구현
- 드랍 아이템 상호작용 구현 

등이 있다.

## [프로젝트 기간 : 2021.02 ~ 2021.07]
  - 2021.02 : 아이템 선정 및 팀 결성
  - 2021.03 ~ 2021.05 : 스토리 구상 및 게임 컨셉 설정
  - 2021.04 ~ 2021.06 : 캐릭터, 아이템 컨셉 설정
  - 2021.05 : 컨셉아트 제작
  - 2021.07 : 프로토타입 개발
  - 2021.07 : 팀 해체, 프로젝트 중단.

 # 프로토타입 개발 화면
  <p align="center"><img src = "https://user-images.githubusercontent.com/57585303/150061198-a6dbeab5-f8c4-4c95-8c85-4859fd10adf1.gif"></p>

  - **카메라**
  
    넓은 맵에서 카메라가 플레이어를 추적하도록 만들고, 자연스러운 카메라의 움직임을 Lerp 함수로 표현하였다.
    
  - **점프 시스템**

    벨트스크롤 게임 특성상 2D에서의 가상의 z축(높이)을 표현하기 위해 캐릭터의 발 아래에 Shadow 오브젝트를 만들고 콜라이더를 설정한다. 아바타의 Rigidbody를 Dynamic으로 유지해야 하므로 AddForce 대신 Translate 함수로 점프 시스템을 구현하였다.
    
