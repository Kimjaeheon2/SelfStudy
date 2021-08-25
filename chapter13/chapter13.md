### 자바스크립트의 기능
* 웹의 요소를 제어한다
* 웹 애플리케이션을 만든다
* 다양한 라이브러리를 사용한다

### 웹브라우저\+자바스크립트
* \<script\> 태그로 자바스크립트 작성
* <script src="스크립트 파일경로"></script> : 외부스크립트파일로 연결
##### 예제
```
<body>
  <h1 id="heading">자바스크립트<h1>
    <p id="text">클릭</p>
    <script>
      var heading = document.querySelector('#heading');
      heading.onclick = function(){
      heading.style.color = "red";
      }
      </script>
    </body>
 ``` 
 ### 자바스크립트 용어와 기본 입출력 방법
 * alert(메시지) : 알림창 출력
 * confirm(메시지) : 확인창 출력
 * prompt(메시지) 또는  prompt(메시지, 기본값) : 프롬프트 창에서 입력받기
 * document.write() : 웹브라우저 화면에 출력
 * colsole.log() : 콘솔창에 출력

### 자바스크립트 스타일 가이드
1.코드를 보기좋게 들여쓰기한다
2.세미콜론으로 문장을 구분한다
3.공백을 넣어 읽기 쉽게 작성한다
4.소스코드를 잘설명하는 주석을 작성한다
5.식별자는 정해진 규칙을 지켜 작성한다
6.예약어는 식별자로 사용할 수 없다
