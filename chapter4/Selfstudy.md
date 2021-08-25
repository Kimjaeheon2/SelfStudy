# 텍스트 입력하기



\<hn>제목\</hn\> : 제목을 나타냄, n의 자리에는 1~6의 숫자가 들어가며 크기별로 표시가능

 \<p\> 내용 \</p\> : 택스트 단락 만들기

\<br\> : 줄바꾸기

 \<blockquote\> 인용문 \</blockquote\> : 인용할 때 사용

\<strong\> 내용 \</strong\> : 텍스트를 굵게 표시

 \<b\> 내용 \</b\> : 텍스트를 굵게 표시

\<em\> 내용 \</em\> : 기울임

\<i\> 내용 \</i\> : 기울임  

\##### 예제

<h1>레드향</h1>

<h2>레드향 샐러드 레시피</h2>

<i>비타민</i>

<b>감기예방</b>



#목록 만들기

\<ol\>,\<li\>태그 : 순서 있는 목록을 만듬
 \<ul\>,\<li\>태그 : 순서 없는 목록을 만듬
 \<dl\>,\<dt\>,\<dd\>태그 : 설명 목록을 만듬

##### 예제
```
<ol>
  <li> 첫번째 문장 </li>
  <li> 두번째 문장 </li>
  <li> 세번째 문장 </li>
</ol>
<ul>
  <li> 첫번째 문장 </li>
  <li> 두번째 문장 </li>
  <li> 세번째 문장 </li>
</ul>
```

<ol>
  <li> 첫번째 문장 </li>
  <li> 두번째 문장 </li>
  <li> 세번째 문장 </li>
</ol>
<ul>
  <li> 첫번째 문장 </li>
  <li> 두번째 문장 </li>
  <li> 세번째 문장 </li>
</ul>

# 표 만들기

\<table\>,\<caption\>태그 : 표만들기
\<tr\>,\<td\>,\<td\>태그 : 행과 셀을 만듬
\<rowspan\>,\<colspan\>태그 : 행이나 열을 합침
\<col\>,\<colgroup\>태그 : 열을 묶어줌

```
<table>
  <caption>표 테스트</caption>
  <tr>
    <th>가</th>
    <th>나</th>
    <th>다</th>
  </tr>
   <tr>
    <td>가-1</td>
    <td>나-1</td>
    <td>다-1</td>
  </tr>
   <tr>
    <td>가-2</td>
    <td>나-2</td>
    <td>다-2</td>
  </tr>
 </table>
 ```
```

<table>
  <caption>표 테스트</caption>
  <tr>
    <th>가</th>
    <th>나</th>
    <th>다</th>
  </tr>
   <tr>
    <td>가-1</td>
    <td>나-1</td>
    <td>다-1</td>
  </tr>
   <tr>
    <td>가-2</td>
    <td>나-2</td>
    <td>다-2</td>
  </tr>
 </table>

```
<table>
  <caption>병합 테스트</caption>
  <tr>
    <th>가</th>
    <th>나</th>
    <th>다</th>
  </tr>
   <tr>
    <td rowspan="2">행 합침</td>
    <td colspan="2">열 합침</td>
   </tr>
   <tr>
    <td>나-2</td>
    <td>다-2</td>
  </tr>
 </table>
 ```
```



<table>
  <caption>병합 테스트</caption>
  <tr>
    <th>가</th>
    <th>나</th>
    <th>다</th>
  </tr>
   <tr>
    <td rowspan="2">행 합침</td>
    <td colspan="2">열 합침</td>
   </tr>
   <tr>
    <td>나-2</td>
    <td>다-2</td>
  </tr>
 </table>

# 이미지 삽입하기
* \<img src="이미지 파일 경로" alt = "대체용 텍스트"\>

##### 예제
<img src="" alt = "그림">



# 오디오와 비디오 삽입하기
* \<object width="너비" height="높이" data="파일"\>\</object\> 다양한 멀티미디어 파일 삽입

* \<audio src="오디오 파일 경로"\>\</audio> : 오디오 파일 삽입

* \<video src="오디오 파일 경로"\>\</video> : 비디오 파일 삽입

  

  

# 하이퍼링크 삽입하기

* \<a href="링크할 주소"\>텍스트 또는 이미지\</a\>

##### 예제

<a href="https://www.google.co.kr/">구글 홈페이지</a>  
<a href="https://www.google.co.kr/"><img src="" alt="구글 로고"></a>

