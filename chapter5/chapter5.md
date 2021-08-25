# 폼 삽입하기

* \<form[속성="속성값"]/>여러 폼 요소\</form\> : 폼만들기
* \<fieldset\>, \<legend\> : 폼 요소를 그룹으로 묶기
* \<lable\> : 폼 요소에 레이블을 붙임
  * 폼 태그의 속성
    * method : 사용자가 입력한 내용을 서버 쪽 프로그램으로 어떻게 넘겨줄 것인지 지정합니다.
    * name : 자바스크립트로 폼을 제어할 때 사용할 폼의 이름을 지정합니다.
    * action : 폼 태그 안의 내용을 처리해 줄 서버 프로그램을 지정합니다.
    * target : action 속성에서 지정한 스크립트 파일을 현재 창이 아닌 다른 위치에서 열도록 합니다.
  
  ##### 예제
  ```
  <form action="register.php">
  /*여러 폼 요소*/
  </form>
  ```
  ```
  <form action="">
  <fieldset>
    <legend>상품 선택</legend>
    </fieldset>
  <fieldset>
    <legend>배송 정보</legend>
    </fieldset>
  </form>
  ```
  
  # 사용자 입력을 위한 input 태그
  
  * text : 텍스트 박스를 넣는다
  * password : 비밀번호를 입력 할 필드를 넣는다
  * search : 검색할때 입력하는 필드를 넣는다
  * url : URL주소를 입력할 수 있는 필드를 넣는다
  * checkbox : 주어진 여러 항목 중 2개이상 선택할 수 있는 체크박스를 넣는다
  * radio : 주어진 여러 항목에서 1개만 선택할 수 있는 라디오 버튼을 넣는다
  * number : 숫자를 조절할 수 있는 스핀 박스를 넣는다
  * range : 숫자를 조절할 수 있는 슬라이드 막대를 넣는다
  * date : 사용자 지역을 기준으로 날짜를 넣는다
  * submit : 전송 버튼을 넣는다
  * reset : 리셋 버튼을 넣는다
  * image : submit버튼 대신 사용할 이미지를 넣는다
  * button : 일반 버튼을 넣는다
  * file : 파일을 첨부할 수 있는 버튼을 넣는다
  * hidden : 사용자에게 보이지 않지만 서보로 넘겨주는 값이 있는 필드를 만든다
  
  # 예제
  ```
  <fieldset>
  <legend>상품 선택</legend>
  <p><b>주문할 상품을 선택해 주세요</b></p>
  <label><input type "checkbox" value="s_3">선물3키로</label>
  <label><input type "checkbox" value="s_5">선물5키로</label>
  <label><input type "checkbox" value="f_3">가정3키로</label>
  <label><input type "checkbox" value="f_3">가정5키로</label>
  <p><b>포장 선택</b></p>
  <label><input type "radio" name="gift" value="yes">포장함</label>
  <label><input type "radio" name="gift" value="no"">포장안함</label>
  </fieldset>
  ```
### input 태그의 주요 속성
   * autofocus : 자동으로 입력 커서를 갖다놓음
   * placeholder : 힌트를 표시해준다
   * readonly : 읽기 전용 필드를 만들어준다
   * required : 필수 입력 필드를 지정한다

### 폼에서 사용하는 여러 태그
   * textarea : 여러 줄을 입력하는 텍스트 영역
   * select,option : 드롭다운 목록을 만들어줌
   * datalist,option : 데이터 목록을 만들어줌
   * button : 버튼을 만들어줌
 
  
