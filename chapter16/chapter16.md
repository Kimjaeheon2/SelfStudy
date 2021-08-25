### 객체
* 자바스크립트에서 객체는 프로그램에서 인식할 수 있는 모든 대상을 가리킨다
* 문서 객체 모델(DOM): 웹 문서 자체도 객체이고 그 안에 삽입되어 있는 이미지와 링크, 텍스트 필드 등도 모두 객체이다.
* 브라우저 관련 객체 : 웹 브라우저에서 사용하는 정보도 객체로 나타낼 수 있다
* 내장 객체 : 웹 프로그래밍을 할 때 자주 사용하는 요소는 자바스크립트 안에 미리 객체로 정의되어 있는데, 이를 내장객체라고 한다.
* 객체 인스턴스 만들기
  * new 객체명
* 자바스크립트의 내장 객체
  * Array : 배열을 다루는 객체
    * var numbers = new Array(); // 배열의 크기를 정하지 않음  
    * var numbers = new Array(4); // 배열의 크기를 정함
    * join() : 배열안의 요소끼리 합침
    * push(), unshift() : 새로운 요소 추가
    * pop(), shift() : 배열에서 요소를 꺼냄
    * splice() : 원하는 위치에 요소를 추가,삭제
    * slice() : 기존 배열을 바꾸지 않으면서 요소를 꺼냄
  * Date : 날짜와 시간정보를 나타낸다
    * new Date(); // 현재날짜 나타내기
    * getFullYear() : 연도를 4자리수로 표시
    * getDate() : 1~31사이의 숫자로 1을 표시
    * getMonth() : 0~11 사이의 숫자로 월 표시 0부터 1월이 시작되고 11은 12월이다
  * Math : 수학관련 메서드가 많지만 무작위수가 필요하거나 반올림 해야하는 경우에도 사용
    * E : 오일러 상수
    * PI : 원주율
    * SQRT2 : 루트2

### 브라우저 관련 객체
* window : 브라우저 창이 열릴 때마다 하나씩 만들어짐
* document : 웹 문서마다 하나씩 있으며 \<body\> 태그를 만나면 만들어진다
* navigator : 현재 사용하는 브라우저의 정보가 들어 있습니다.
* history : 현재 창에서 사용자의 방문 기록을 저장합니다.
* location : 현재 페이지의 URL정보가 담겨있다
* screen : 현재 사용하는 화면 정보를 다룬다

##### 예제
```
var now = new Date();
document.write("현재 시각은"+ now);
```
```
<script>
  var now = new Date("2020-10-15");
  var firstDay= new Date("2020-10-01");
  var toNow = now.getTime();
  var toFirst = firstDay.getTime;
  var passedTime = toNow-toFirst;
  
  passedTime = Math.round(passedTime/(100*60*60*24));
  document.querySelector("#result").innerText = passedTime;
  </script>

