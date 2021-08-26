### 문서 객체 모델 알아보기

* 자바스크립트를 이용하여 웹 문서에 접근하고 제어할 수 있도록 객체를 사용해 웹 문서를 체계적으로 정리하는 방법
* DOM 트리란요소의 내용을 부모와 자식 구조로 표히사여 나무형태가 되도록 하는것
    * node : DOM트리에서 가지가 갈라져 나간 항목
    * root : DOM트리의 시작부분인 HTML노드를 뿌리에 해당한다 해서 루트노드라고한다
    * 기본원칙
      1.모든 HTML태크는 요소노드입니다.   
      2.HTML 태그에서 사용하는 텍스트 내용은 자식 노드인 텍스트(text) 노드이다.   
      3.HTML 태그에 있는 속성은 자식 노드인 속성 노드이다.   
      4.주석은 주석 노드이다.   
### DOM에 접근하기
* id 선택자로 접근하는 getElementById()메서드
* class값으로 접근하는getElementByClassName()메서드
* 태그 이름으로 접근하는 getElementByTagName()메서드
* 다양한 방법으로 접근하는 querySelector(), querySelectorAll() 메서드
* 웹 요소의 내용을 수정하는 innerText,innerHtml프로퍼티
* 속성을 가져오거나 수정하는 grtAttribute(), setAttribute() 메서드


### DOM에서 이벤트 처리하기
* DOM의 event 객체
  * altkey : 이벤트가 발생할 때 알트를 눌렀는지 여부를 boolean값으로 반환
  * button : 마우스에서 누른 버튼의 키값을 반환합니다.
  * charCode : keypress이벤트가 발생할 때 어떤 키를 눌렀는지 유니코드값으로 반환
  * clientX : 이벤트가 발생한 가로 위치 반환
  * ctrlKey : 벤트가 발생할 때 컨트롤키를 눌렀는지 여부를 boolean값으로 반환
  * pageX : 현재 문서 기준으로 이벤트가 발생한 가로 위치를 반환한다.
  * screenX : 현재 화면 기준으로 이벤트가 발생한 가로 위치를 반환한다.
  * shiftkey : 이벤트가 발생할 때 쉬프트키를 눌럿는지 여부를 boolean값으로 반환
  * target : 이벤트가 최초로 발생한 대상을 반환
  * timeStamp : 이벤트가 발생한 시간을 반환
  * stpe : 발생한 이벤트 이름을 반환합니다
  * which : 키보드와 관련된 이벤트가 발생할 때 키의 유니코드값을 반환합니다
  * preventDefault() : 이벤트를 취소할 수 있는 경우에 취소한다
* CSS 속성에 접근하기
  * document.getElementById("desc").style.color ="blue";

### DOM에서 노드 추가.삭제하기
* 노드리스트란 DAM에 접근 할 때 querySelectorALL()메서드를 이용해 노드를 한거번에 여러개 가조여고 이것을 저장한것이 노드리스트이다.
1 createElement() : 요소 노드 만들기
2 createTextNode() : 텍스트 노드 만들기
3 appendChild() : 자식 노드 연결하기

##### 예제
```
<button onclick=:inntext()">innerText로 표시하기</button>
<button onclick:"innhtml()">innerHTML로 표시하기</button>
                           <h1>현재 시각:</h1>
                           <div id="current"></div>
                                            
                                            <script>
                                            
                                            var now= new Date();
                                            function inntext(){
                                            document.getElementById("current").innerText=now;
                                                                             }
                                                                             fuunction innhtml(){
                                                                             document.getElementById("current").innerHTML="<em>"+now+"</em>";
                                                                             }
                                                                             </script>
                                                                             ```
                        
                                                      
