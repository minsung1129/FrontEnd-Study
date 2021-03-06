# CSS 반응형 디자인과 미디어 쿼리
### 1.반응형 디자인
CSS에서 반응형 디자인이란, 웹 페이지에 접속한 디바이스의 종류에 따라 웹 페이지의 크기를 재조정하거나 재조정된 웹 페이지에 따라 변화하는 요소들을 뜻한다. 반응형 웹이 필요한 이유는 최근 PC뿐만 아니라 모바일을 통한 웹 접속이 많아졌기 때문이다. 
### 2.미디어 쿼리
Media Query는 이러한 반응형 웹을 디자인하기 위한 기법 중 하나이다.
```
@media only all and (조건문) {
    실행문
}
```
* @media : 미디어 쿼리의 시작을 알린다.
* only : 미디어 쿼리를 지원하는 사용자에게만 해석하라는 뜻한다.
* all : 미디어 쿼리를 해석해야 할 대상 미디어를 뜻한다. all 대신 screen을 넣게 되면 screen만 해석하게 된다.
* 실행문 : 조건문을 만족했을 때 실행되는 CSS이다.
#### 2-1.조건문
미디어 쿼리의 실행문을 실행할 때의 조건을 나타낸다.
```
max-width : 780px;
```
위와 같은 조건이 존재한다면 '뷰포트의 너비가 780px보다 작을 때'를 뜻한다. 조건문에 사용할 수 있는 Feature들은 다음과 같다.
* width/height : 뷰포트의 너비/높이
* device-width/device-height : 스크린의 너비/높이
* orientation : 뷰포트의 가로 모드/세로 모드
* aspect-ratio : 뷰포트의 비율(너비/높이)
* device-aspect-ratio : 스크린의 비율(너비/높이)
* color : 색상의 bit 수
* grid : 출력 장치가 grid인가
