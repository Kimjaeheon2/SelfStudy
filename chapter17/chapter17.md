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
                        
                                                      
