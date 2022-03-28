# SCHS Programming Class Note
#### date : 2022-03-29
### lecture title : 웹 브라우저와 웹서버, HTML CSS JAVASCRIPT
* * *


#### keywords
* 웹 브라우저
    - 웹 브라우저란 무엇인가

    정의된 규칙에 따라 작성된 파일을 불러다가 화면에 그려주고, 사용자가 발생시킨 이벤트(마우스 클릭, 이동 등)에 따라 동작시켜주는 응용 프로그램<br/><br/>
    여기에 정의된 규칙에 따라 작성된 파일이 **HTML**파일이다(Hyper Text Markup Language).<br/>이 파일은 웹문서라고도 부른다.

    - 웹 브라우저의 종류

    <pre>Internet Explorer, Edge, Chrome, Opera, Safari, FireFox 등...</pre>

* HTML5
    - HTML 파일의 정의 규칙

    HTML 규칙에 따라 작성된 파일은 웹브라우저에서 읽어들여서 화면에 그려준다.<br/>
    이는 **태그**라는 작성방식을 사용해 작성하게 된다.<br/><br/>

    - HTML 파일 구조(가장 최신버전인 HTML5 규칙을 적용)
    텍스트 형태로 작성하며 구조는 아래와 같다
   ```HTML
    <!DOCTYPE html>
    <html lang="ko">
        <head>
            <meta charset="UTF-8">
            <title>HTML 문서</title>
        </head>
        <body>
            <!--이 태그는 주석을 의미합니다. 초록색이죠? 이 부분은 화면에 나타나지 않는 첨언용입니다.-->
            <h1>프런트엔드 웹 개발</h1>
            <hr>
            <p>태초에 말씀이 계셨고 그 말씀이 하나님과 함께 계셨으니 그 말씀은 하나님이셨느니라.</p>
            <p>요한복음 1:1</p>
        </body>
    </html>
   ```
    - 실습<br/>
    1. github desktop에서 current repository를 자신의 repository로 변환하여, VS Code에서 열 것.
    2. 열린 VS Code에서 practice2 디렉토리를 생성하고, 해당 폴더 안에 html파일 확장자를 만들 것.
    3. 위 코드를 ctrl+c, v 하지말고 직접 타이핑하여 작성해 볼 것.
    4. 자신이 저장한 로컬 repository 디렉토리에서 작성한 HTML 코드를 더블클릭하여 웹브라우저(chrome)에서 동작시켜 볼 것.
    <br/>
    <br/>
    
    - 실습2<br/>
    1. chrome > 우상단 더보기버튼(점세개버튼) > 도구 더보기 > 개발자도구를 눌러볼 것
    2. 나타난 개발자 도구에서 source 탭을 열어볼 것. 거기에 자신의 html파일을 확인 할 것.
    3. VS Code에서 html 코드에 있는 h1태그 내용을 마음대로 수정해볼 것. title 내용도 수정해볼 것.
    4. 수정 후 웹브라우저의 F5키를 눌러서 새로고침 해볼 것.
    <br/>
    <br/>

    - HTML 작성 규칙에 대한 설명<br/>
    ```HTML
    <!--해당라인은 현재 문서가 HTML5 작성 규칙으로 텍스트 타이핑을 한 파일임을 나타내줍니다.-->
    <!DOCTYPE html>
    ```

    태그는 기본적으로 시작태그와 끝태그가 있습니다.
    ```HTML
    <!--해당 태그는 html 내용을 시작하는 것입니다. 태그 작성규칙은 기본적으로 시작과 끝이 슬래시 태그로 구분되고
    태그 사이에 텍스트 내용이나, 다른 태그들을 더 기입할 수 있습니다.
    아래 태그는 html 태그입니다.
    -->
    <html>~</html>
    ```

    ```HTML
    <!--html의 태그 내에 들어갈 수 있는 태그는 기본적으로 head태그와 body태그가 짝을 이루어 들어갑니다.-->
    <html>
        <head>~</head>
        <body>~</body>
    </html>
    ```

    - head 태그 내용은 무엇인가
    
* * *
#### tasks
* 기본 HTML5 형태 만들기. 반복해서 써넣을 수 있도록
* 크롬 브라우저에서 개발자 콘솔을 열어서 소스 살펴보기