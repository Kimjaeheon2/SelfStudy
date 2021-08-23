### HTML이란?
html 이란 간단히 줄여서 웹 문서를 만드는 언어이다.

### HTML 문서구조
 \<!DOCTYPE html\>로 시작해 \<html\>, \<head\>, \<body\>라는 3개의 영역으로 구성되어 있다.  
 \<!DOCTYPE html\> : 현재 문서가 HTML5언어로 작선한 웹 문서라는 뜻입니다.    
 \<html\> ~ \</html\> : 웹 문서의 시작과 끝을 나타내는 태그입니다.   
 \<head\> ~ \</head\> : 웹 브라우저가 웹 문서를 해석하는 데 필요한 정보를 입력하는 부분입니다.   
 \<body\> ~ \</body\> : 실제로 웹 브라우저 화면에 나타나는 내용입니다.   



### HTML 문서예제

<!DOCTYPE html>
    <html lang="ko">
        <head>
            <meta charset="UTF-8">
            <title>첫 번째 웹 문서 연습</title>
        </head>
        <body>
            <h1>웹 문서 만들기</h1>
        </body>
</html>
html의 기본 구조를 완성한 코드


### 시맨틱 태그란?

html의 태그는 그 이름만 봐도 의미를 알 수 있어 시맨틱 태그라고 합니다. 텍스트 단락을 줄인\<p\> anchor을 줄인 \<a\> 태그 등이 있습니다.


### 시맨틱 태그의 종류

* \<header\> :  헤더 영역을 나타냄
* \<nav> : 네비게이션 영역을 나타냄
* \<main\> : 핵심 콘텐츠를 담음
* \<article> : 독립적인 콘텐츠를 담음
* \<section\>  : 콘텐츠 영역을 나타냄
* \<aside\> : 사이드바 영역을 나타냄
* \<footer\> : 푸터 영역을 나타냄
* \<div> : 여러 소스를 묶음


<!DOCTYPE html>
    <html lang="ko">
<main class="contents">
    <section id="headling">
        <h2>몸과 마음이 치유되는 섬</h2>
    </section>
    <section id="activity">
        <h2>다양한 액티비티가 기다리는 섬</h2>
    </section>
</main>
 </html>
