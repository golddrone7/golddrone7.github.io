# 소나기 게임

<img src="https://github.com/golddrone7/golddrone7.github.io/blob/main/%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8%20%EA%B5%AC%EC%83%81%EB%8F%84/img/sonagi.gif" width="1080" height="720"/>

# 😄소나기 게임에 오신걸 환영합니다!😄
- <a href="https://golddrone7.github.io/">0. 소나기 게임 하러가기</a>
- 협업 프로젝트 2번째!
- <a href="#a">1. 개발 배경</a>
- <a href="#b">2. 개발 목표</a>
- <a href="#c">3. 밴치 마킹</a>
- <a href="#d">4. 개발 환경</a>
- <a href="#e">5. 개발 기간</a>
- <a href="#f">6. 역할 분담</a>
- <a href="#g">7. 개발 내용</a>
- <a href="#h">8. 개발 팀원</a>
- <a href="#i">9. 회고록</a>
- <a href="https://github.com/golddrone7/golddrone7.github.io/blob/main/%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8%20%EA%B5%AC%EC%83%81%EB%8F%84/%EC%86%8C%EB%82%98%EA%B8%B0%20project.pdf">소나기 게임.pdf</a>

---


<div id="a"></div>

## 1. 개발 배경
- 대부분의 타자 연습은 교육용, 프로그램 방식
- 리듬게임처럼 웹으로 즐기는 타이핑 게임을 만들어보고자 개발하였음

<div id="b"></div>

## 2. 개발 목표
- 범용성 : 언제 어디서든 즐길 수 있게 웹 환경 동작 방식
- 편의성 : 사용자 UI, 게임 방법, 눈의 피로를 생각한 색상 배치
- 재미 : 리듬감이 느껴질 수 있도록 애니메이션과 재미 요소를 목표

<div id="c"></div>

## 3. 밴치 마킹

### 산성비 게임
1. 정적인 게임 화면
2. 프로그램 동작
3. 스테이징 방식
4. 오래된 UI/UX
5. 교육 타이핑

### 소나기 게임
1. 동적인 게임 화면
2. 웹 환경 동작
3. 난이도 방식
4. 직관적인 디자인
5. 게임 타이핑


<div id="d"></div>

## 4. 개발 환경
### FrontEnd
- visual studio code, HTML, CSS, JavaScript
### 협업툴
- git, github
- Notion

<div id="e"></div>

## 5. 개발 기간
- `23.03.27` ~ `23.03.31` (월~금)
- `1일차` : 프로젝트 주제 선정 및 기획, Git 저장소 구축
- `2일차` : 게임 레이아웃 로직 구현, 모듈 통합화
- `3일차` : 게임 시작화면, 결과 화면 구현, 애니메이션 및 디자인 작업
- `4일차` : 게임 편의성 부분 개선, 게임 레이아웃 개선
- `5일차` : 게임 전반적인 CSS 수정, project ppt 작성, 마무리 작업
 

<div id="f"></div>

## 6. 역할 분담
- <<b>팀장</b>>송유근 : 레이아웃, 게임 로직 및 알고리즘(충돌, 생성, 난이도, 조건) 
- <<b>팀원</b>>조상천 : 게임 알고리즘(정답 검증 및 결과창), CSS 작업
- <<b>팀원</b>>이상욱 : OPENING 화면 구현, CSS, 애니메이션 효과 작업

<div id="g"></div>

## 7. 개발 내용

### 1. 인트로
<img src="./프로젝트%20구상도/img/인트로.png"/>

- "SONAGI GAME"이 일정한 간격으로 출력
- 4초 후 게임 설정 페이지로 이동

### 2. 게임 설정
<img src="./프로젝트%20구상도/img/../../프로젝트%20구상도/img/게임%20설정.png"/>

- 이름과 난이도를 입력 받음
- 이름을 작성하지 않으면 "GUEST"로 설정
- 난이도는 총 3개가 있음
- easy, normal, hard
- 단어 생성 시간의 차이로 조절하였음

### 3.1 게임 화면
<img src="./프로젝트%20구상도/img/../../프로젝트%20구상도/img/../../프로젝트%20구상도/img/게임화면-1.png"/>

- 게임 방법을 설명해주는 화면
- 게임 준비 버튼을 누르면 게임 시작이 됨
- 자동으로 input창에 focus 설정
- LIFE는 기본적으로 5로 설정하였음

### 3.2 게임 화면
<img src="./프로젝트%20구상도/img/../../프로젝트%20구상도/img/../../프로젝트%20구상도/img/게임화면-2.png"/>

- 오른쪽 상단의 숫자는 콤보
- 단어가 게임 화면 하늘에서 일정한 주기로 떨어짐
- 단어가 바닥에 닿으면 인풋 박스 애니메이션 효과 및 라이프 1 감소
- 단어를 맞추면 콤보가 1 증가 및 애니메이션 효과

### 3.3 게임 화면 
<img src="./프로젝트%20구상도/img/../../프로젝트%20구상도/img/../../프로젝트%20구상도/img/../../프로젝트%20구상도/img/게임화면-3.png"/>

- 점수는 콤보에 비례하여 단어를 맞출 때 마다 증가
- 단어를 틀리거나 바닥에 충돌하면 콤보 0으로 초기화

 ### 4. 게임 결과
<img src="./프로젝트%20구상도/img/../../프로젝트%20구상도/img/../../프로젝트%20구상도/img/../../프로젝트%20구상도/img/../../프로젝트%20구상도/img/결과창.png"/>

- 맞춘 정답을 결과에 표시
- 넘칠 경우 스크롤이 생김
- 이름, 최고 콤보 기록, 점수 표시
- 다시하기 버튼 기능 구현
- 게임 설정 화면으로 되돌아감

<div id="h"></div>

## 8. :family: 개발 팀원 소개

|  <a href="https://github.com/golddrone7"><img src="./프로젝트/../프로젝트%20구상도/img/유근.png" alt="유근" style="zoom: 25%;" width=400 /></a> |  <a href="https://github.com/highsky134"><img src="./프로젝트/../프로젝트%20구상도/img/상천.png" alt="상천" style="zoom: 25%;" width=400 /></a> |  <a href="https://github.com/TTTWIXX"><img src="./프로젝트/../프로젝트%20구상도/img/상욱.png" alt="상욱" style="zoom: 25%;" width=400 /></a> |
 | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| **송유근**<br />(팀장)                             | **조상천**<br />(팀원)                       | **이상욱**<br />(팀원)                       | 
<div id="i"></div>

## 9. 회고록

| 이름   | 내용                                                         |
| ------ | ------------------------------------------------------------ |
| 송유근 | - 소나기 게임 프로젝트를 무사히 끝마쳤습니다. 프로젝트를 경험을 하면서 협업이 무엇인지 깨달았습니다. 주제 선정 및 기획부터 매일매일 1~2시간씩 토론 회의를 진행했습니다. 처음에는 문서 없이 생각만으로 아이디어를 말하기엔 한계가 있었습니다. 문서를 작성을 해서 개발 방향과 피드백을 받았습니다. 팀원분들이 너무 적극적이고 맡은 역할들을 완수를 해준 덕분에 프로젝트 내내 화기애애한 분위기로 즐겁게 개발을 했습니다.<br/> - 몇 가지 경험을 하면서 <b>어려웠던 점</b>은 역할 분배, 충돌 처리, 디자인, 모듈화 작업입니다. 역할 분배는 기능들을 적절하게 나눕니다. 충돌 처리는 JS에는 이벤트 처리가 한정적이어서 애니메이션 시간과 콜백함수를 써서 해결을 했습니다. 디자인 작업 부분은 리듬 게임들을 많이 참고를 했습니다. 모듈화 작업은 각자 작업한 코드를 하나로 합치는 작업이 어려웠습니다. Github 전략에 대해서도 많이 배울 수 있는 좋은 경험이었습니다.  |
| 조상천 | 123 |
| 이상욱 | 1. 어려웠던점<br/>js를 배우고 처음으로 했던 프로젝트이다. git관리부터 시작하여(branch생성, merge시 충돌...), 역할 분담, 변수 통일 등 새로운것 투성이였다. 수업시간에 눈으로 보고 생각하는 것과는 달리 직접 머리속에 있는 생각들은 코드를 통해 구현해 나가는 것이 정말 어려웠다. 특히 충돌감지 부분에서 수업시간에 배운 내용으로 작성하는데 있어 많은 어려움을 겪었다. <br/>2. 재미있었던점 <br/> 다양한 animation 효과를 통해 내가 원하는 효과를 찾아가는 점이 흥미로웠다. 특히 js코드를 통해 내가 원하는 값을 받을때마다 효과가 나타나게 할 수 있다는 점이 재미있었다. 분담하여 작성했던 코드를 합쳐 하나로 만들었을때의 성취감을 느꼈다. 조원들이 맡은 파트를 하나로 병합하여 실행해봤을 때 퍼즐이 완성되는 느낌을 받았다. <br/> 3. 배웠던점</br> 정말 단순한 게임이라고 생각했지만 생각보다 고려해야할 점이 굉장히 많았다. 기본적인 git 사용부터 시작하여, 역할분담, 조원간 커뮤니케이션, 기본적인 css(프로그램 컨셉, 이미지).js를 이용한 코드 작성 등 많은 것을 시도하였고 경험하는 계기가 되었다. 특히 조원들의 프로젝트 진행방법 (md작성, 계획서 작성, git 사용법(병합용 branch 생성), code 사용법)에 대해 많은 경험을 할 수 있었다. |

