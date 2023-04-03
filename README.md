# 소나기 게임

<img src="https://github.com/golddrone7/golddrone7.github.io/blob/main/%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8%20%EA%B5%AC%EC%83%81%EB%8F%84/img/sonagi.gif" width="1080" height="720"/>

## 1. 개요 
- (임시) 신조어 암기 게임(소나기)11

## 2. 게임 흐름 
- 인트로 -> 사용자 입력 -> 게임 진행 ->  결과 확인 및 게임당 점수 기록, 단어 뜻 보여주기 

## 3. 게임 흐름 세부
- [공통사항] 라이프 수 5개
- 3-0. 인트로 : 간단한 게임 스토리!!
-  3-1. 시작 화면 : 큰 화면에 사용자를 입력 받아 게임을 시작 // 반투명 화면에 입력 창과 그 뒤로 게임 페이지가 비춰짐
- 3-2. 게임 시작  
-   3-2-1 : 3단계의 난이도 설정 페이지 존재 설정 후 게임 실행 
  	    게임 난이도 : 단어 떨어지는 속도 (1, 1.5, 2)    => (추후) 게임 화면 단어수 증가
   
- 3-3. 게임 진행 - [준비 : 원하는 만큼의 단어를 배열에 넣어 둬야 함]   
    1. 게임 박스 최상단에서 단어가 아래로 내려옴
    2. 박스 하단에 입력창이 주어지고 사용자가 입력
    3. 정답 검증
   	    - 3-1. 정답 시 해당 문구 삭제 및 점수 증가, 콤보 횟수 +1 증가
		(추후) 해당 문구 삭제부분을 애니메이션 효과를 넣으면 좋을 것 같아요! 
   	    - 3-2. 오답 시 콤보 횟수 0
	    - 타이핑 (공통사항) : 엔터를 치면 해당 input 값을 ""로 초기화

    4. 목표 점수 도달 또는 목숨이 0이 되면 게임 종료
    5. 해당하는 점수를 보여주는 점수 기록 페이지 보여줌
        - 5-1. 결과 확인 및 게임당 점수 기록, 단어 뜻 보여주기, "다시하기" 버튼
	    - "다시하기" 버튼 누르면 3-1로 진행
   

### 목표점수 50점 (임시)
- 10콤보 시 : 콤보의 box-shadow 값의 블러를 증가시킴 (자유로운 애니메이션 효과)
- 20콤보 시 : 콤보의 box-shadow 값의 블러를 증가시킴
- 30콤보 시 : 콤보의 box-shadow 값의 블러를 증가시킴
- (추신)콤보 맞출 때마다 통통 튀는 효과를 줘도 좋을것 같아요    




### 고려 해야 할점
1. 문구가 등장하는 박스 상단을 어떻게 배치해야 하는가?  
2. 놓쳤을 때 어떻게 해야 하는가? 	
   기준점에서 사라지게 해야되는가? 기준점 약간 위에서 opacity값을 서서히 낮추면서 자바스크립트 element로 삭제하면 될 것같아요
   그냥 숨기면(z-index) 될까?


### 향후 개발 ( 현재 하기 어렵거나 애매한 부분 )
1. 게임 시작 전 사용자를 입력받아 게임 종료 후 점수별 랭킹 보여주기
2. 난이도 대신 게임 모드 설정 : 한글, 영어, 사칙연산







## 참고사항!
### 24가지 JavaScript 프로젝트
https://mikkegoes.com/javascript-projects-for-beginners/
### 40가지 JavaScript 프로젝트
https://www.freecodecamp.org/news/javascript-projects-for-beginners/
