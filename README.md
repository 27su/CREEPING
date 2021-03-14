# CREEPING
1. git clone을 합니다   
2. creeps.py를 실행합니다 [ 실행 명령어 : python creeps.py ]   

1) 참고하는 OSS 출처:
https://github.com/eliben/code-for-blog/tree/master/2009/pygame_creeps_game    
   
   
2) 『CREEPING』 프로젝트에서 사용하는 기술   
- 프로그래밍 언어: Python    
– OS: Ubuntu, Linux     
- 오픈소스 기술: Pygame, Github      
   
   
3) 추진목표 : Python과 Pygame을 이용한 게임의 추가기능 구현을 목적으로 한다. 오픈소스를 분석하고 이를 활용해 개별적으로 내용을 추가하여 『CREEPING』을 만든다. 완성된 『CREEPING』은 일시정지 버그가 수정되고, 기존의 기능에 ‘게임 재시작 기능’과 ‘획득한 점수화면’이 추가된 게임이다.    
   
      
4) 프로젝트에서의 담당 업무        
– pathfinder.py, priorityqueueset.py, widgets.py, gridmap.py 코드 분석   
- 일시정지 기능과 획득한 점수 표시 기능 구현   
- 제안서·보고서 작성, 중간발표, 최종 발표 자료 수정, 최종 발표   
   
   
5) 추가 기능   
- 일시정지 버그 수정 : 게임을 일시 정지했을 때 사용자가 실행한 동작이 게임에 영향을 주지 않게 수정한다.    
설명: 함수 mouse_click_event에 if not self.game.paused를 추가하여 게임이 정지 상태가 아닐 때에만 mouse_click_event의 기존 코드가 실행되도록 수정하였다. 
   
-  재시작 버튼 : 게임이 다 끝나고 재시작을 할 수 있게 하는 기능을 구현한다.   
설명: r을 누르면 게임을 재시작 할 수 있도록 elif문 코드를 추가하였다.   
   
- 점수화면 : 점수를 얼마나 획득했는지 화면에 표시하는 기능을 구현한다.   
설명: 게임 Score 확인을 위해 Game 클래스에 score 인스턴스 변수를 추가하였다. score 변수는 __init__함수에서 0으로 초기화 된다. 그리고 creeps가 사용자의 이벤트 클릭에 의해 _die()가 호출될 때 마다 socre의 값을 1씩 증가하도록 구현하였다. 또한 게임 score 점수는 남은 creeps의 수를 표시하는 상자에서 확인 할 수 있도록 코드를 수정하였다.   
   
