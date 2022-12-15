HTML이란?

HTML(Hypertext Markup Language,하이퍼텍스트 마크업 언어)

프로그래밍 언어는 아니고, 

우리가 보는 웹페이지가 어떻게 구조화되어 있는지 브라우저로

하여금 알 수 있도록 하는 마크업 언어( makeup lnaguage )입니다.

markup language : 태그 등을 이용하여 문서 혹은 데이터의 구조를 기록하는 언어

HTML은 elements 로 구성되어 있으며, 

이들은 적절한 방법으로 나타내고 실행하기 위해

각 컨텐츠의 여러 부분들을 감싸고 마크업 합니다.

tags 는 웹 상의 다른 페이지로 이동하게 하는 하이퍼링크 내용들을 생성하거나, 

단어를 강조하는 등의 역할을 합니다. 

​

웹사이트 제작시 고려사항

1.웹 표준

(웹 사이트를 작성할 때 따라야 하는 공식 표준이나 기술 규격)

2.웹 접근성

(장애의 여부와 상관 없이 모두가 웹사이트를 이용할 수 있게 하는 방식 )

3.크로스 브라우징

모든 브라우저 또는 기기에서 사이트가 제대로 작동하도록 하는 기법

​

HTML 태그 구성 요소

​


1. 여는 태그(Opening tag): 이것은 요소의 이름과(이 경우 p), 열고 닫는 꺽쇠 괄호로 구성

요소가 시작(이 경우 단락의 시작 부분)부터 효과가 적용되기 시작합니다.

2. 닫는 태그(Closing tag): 이것은 요소(element)의 이름 앞에 슬래시(/)가 있는것을 제외하

면 여는 태그(opening tag)와 같습니다. 

이것은 요소의 끝(이 경우 단락의 끝 부분)에 위치합니다. 

닫는 태그를 적어주지 않는 것은 흔한 초심자의 오류이며, 

이것은 이상한 결과를 낳게됩니다.

3. 내용(Content): 요소의 내용이며, 이 경우 단순한 텍스트이다.

4. 요소(Element): 여는 태그, 닫는 태그, 내용을 통틀어 요소(element)라고한다.

​

​

<h1>–<h6>: HTML 구획 제목 요소

HTML  <h1> – <h6> 요소는 6단계의 구획 제목을 나타냅니다. 구획 단계는 <h1> 이 가장 높

고 <h6> 은 가장 낮습니다.

특성

<h1> - <h6> 요소는 전역 특성만 포함합니다.

전역 특성(Global attributes) : 모든 HTML에서 공통으로 사용할 수 있는 특성입니

다. 그러나 일부 요소에는 아무런 효과도 없을 수 있습니다. 

​

예제)

1. 모든 제목 단계 

<h1>Heading level 1</h1>

<h2>Heading level 2</h2>

<h3>Heading level 3</h3>

<h4>Heading level 4</h4>

<h5>Heading level 5</h5>

<h6>Heading level 6</h6>

​

<a>

HTML  <a> 요소(앵커 요소)는 href 특성을 통해 다른 페이지나 같은 페이지의 어느 위치, 파

일, 이메일 주소와 그 외 다른 URL로 연결할 수 있는 하이퍼링크를 만듭니다.  <a> 안의 콘텐츠

는 링크 목적지의 설명을 나타내야 합니다.

예제)

1. URL로 연결

<a href="https://www.google.com">​ Sample </a>

2. 이메일 주소로 연결

사용자의 이메일 프로그램을 통해 새로운 메일을 보낼 수 있는 링크를 생성하려면 

mailto: 스킴을 사용

<a href="mailto:nowhere@mozilla.org">Send email to nowhere</a>

​

<br>: 줄바꿈 요소

HTML  <br> 요소는 텍스트 안에 줄바꿈(캐리지 리턴)을 생성합니다. 주소나 시조 등 줄의 구분

이 중요한 내용을 작성할 때 유용합니다.

예제)

Mozilla Foundation<br>

1981 Landings Drive<br>

Building K<br>

Mountain View, CA 94043-0801<br>

USA

​

<table>

HTML  <table> 요소는 행과 열로 이루어진 표를 나타냅니다.

예제

1. 연습

<table>

     <thead>

          <tr>

              <th colspan="2">The table header</th>

         </tr>

    </thead>

    <tbody>

         <tr>

             <td>The table body</td>

             <td>with two columns</td>

       </tr>

  </tbody>

</table>

<col>

HTML  <col> 요소는 표의 열을 나타내며, 열에 속하는 칸에 공통된 의미를 부여할 때 사용합니

다. 

​

<table>

     <caption>Superheros and sidekicks</caption>

     <colgroup>

         <col>

         <col span="2" class="batman">

         <col span="2" class="flash">

     </colgroup>

     <tr>

         <td> </td>

         <th scope="col">Batman</th>

         <th scope="col">Robin</th>

         <th scope="col">The Flash</th>

         <th scope="col">Kid Flash</th>

   </tr>

   <tr>

       <th scope="row">Skill</th>

       <td>Smarts</td>

       <td>Dex, acrobat</td>

       <td>Super speed</td>

       <td>Super speed</td>

 </tr>

</table> 

속성(Attributes)

속성은 요소에 실제론 나타내고 싶지 않지만 추가적인 내용을 담고 싶을 때 사용합니다. 위에는

나중에 스타일에 관련된 내용이나 기타 내용을 위해 해당 목표를 구분할 수 있는 class 속성을

부여했습니다.

<p class="editor-note">My cat is very grumpy</p>

속성을 사용할 때에는 아래 내용을 지켜야 합니다:

1. 요소 이름 다음에 바로 오는 속성은 요소 이름과 속성 사이에 공백이 있어야 되고, 

하나 이상의 속성들이 있는 경우엔 속성 사이에 공백이 있어야 합니다

2. 속성 이름 다음엔 등호(=)가 붙습니다

3. 속성 값은 열고 닫는 따옴표로 감싸야 합니다

​

​

class

전역 특성은 공백으로 구분한 요소 클래스의 목록으로, 대소문자를 구분하지 않습니다. 클래스

는 CSS나JavaScript에서 클래스 선택자나 DOM 메서드의

 document.getElementsByClassName()  (en-US)과 

같은 메서드를 통해 요소에 접근할 수 있는 방법입니다 

예제

<p>Narrator: This is the beginning of the play.</p>

<p class="note editorial">Above point sounds a bit obvious. Remove/rewrite?</p>

<p>Narrator: I must warn you now folks that this beginning is very exciting.</p>

<p class="note">[Lights go up and wind blows; Caspian enters stage right]</p>

.note {

    font-style: italic;

    font-weight: bold;

}

.editorial {

     background: rgb(255, 0, 0, .25);

     padding: 10px;

}

.editorial:before {

     content: 'Editor: ';

}

​

id

전역 특성은 문서 전체에서 유일한 고유식별자(ID)를 정의합니다

고유식별자의 목적은 프래그먼트 식별자를 사용해 요소를 가리킬 때와 

스크립트 및 스타일 적용 시 특정 요소를 식별하기 위함입니다

예제)

<p>A normal, boring paragraph. Try not to fall asleep.</p>

<p id="exciting">The most exciting paragraph on the page. One of a kind!</p>

#exciting {

       background: linear-gradient(to bottom, #ffe8d4, #f69d3c);

       border: 1px solid #696969;

       padding: 10px;

       border-radius: 10px;

       box-shadow: 2px 2px 1px black;

}

​

#exciting:before {

      content: " i ";

      margin-right: 5px;

}

​

style

style 전역 특성은 요소에 적용할 CSS 스타일 선언을 담습니다

 스타일은 별도의 파일에 정의하는 것이 권장된다는 점을 참고

이 특성과 <style> 요소는 주로 테스트 등 빠른 스타일링을 위한 목적으로 사용됩니다

예제)

<div style="background: #ffe7e8; border: 2px solid #e66465;">

      <p style="margin: 15px; line-height: 1.5; text-align: center;">

          Well, I am the slime from your video<br>

          Oozin' along on your livin' room floor.</p>

</div>

​

​

title 

전역 특성은 요소와 관련된 추가 정보를 제공하는 텍스트를 나타냅니다

예제)

<p>Use the <code>title</code> attribute on an <code>iframe</code> to clearly identify the

     content of the <code>iframe</code> to screen readers.</p>

<iframe title="Wikipedia page for the HTML language"

       src="https://en.m.wikipedia.org/wiki/HTML"></iframe>

<iframe title="Wikipedia page for the CSS language"

      src="https://en.m.wikipedia.org/wiki/CSS"></iframe>

iframe {

      height: 200px;

     margin-bottom: 24px;

     width: 100%;

​

}
