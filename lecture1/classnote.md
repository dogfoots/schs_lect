# SCHS Programming Class Note
#### date : 2022-03-22
### lecture title : 개발환경 세팅
* * *


#### keywords
* 프로그래머
    - 프로그래머란

        <pre>컴퓨터가 알아들을 수 있는 [주어진 명령어]를 이용하거나 [명령어를 직접 만들어] 원하는 요구사항에 맞춰<br/>컴퓨터의 [하드웨어/소프트웨어를 동작]시켜주는 사람</pre>

    - 실무에서 프로그래머

        현업의 프로그램 개발은 일반적으로 아래 단계를 따른다.
        1. 기획, 설계 - 기획자
        2. 디자인 - 디자이너
        3. **개발(실제적인 코딩) - 개발자**   
        <br/>
        <pre>그러나 내가 개발자이기 때문에, 기획과 디자인 단계에서 무조건 배제되지는 않는다.<br/>왜냐하면 결국 실제 컴퓨터의 화면 상에서 구현 가능한지,<br/>기술적인 관점에서 의견을 제시해줘야하기 때문이다.</pre>

    - 프로그래머 종류

        국가에서 구분한 직무는 '응용 S/W 프로그래머'와 같은 말로 불린다.
        1. Windows 응용 프로그램 개발자
        2. Mac 응용 프로그램 개발자
        3. iOS 앱 개발자
        4. Android 앱 개발자
        5. 웹 개발자
            1. Front-End 개발자
            2. Back-End 개발자
            3. Full-Stack 개발자   
        6. Embeded 개발자   
        etc...
    
    - 프로그래밍 언어란

        각 시스템에서 자신이 동작시키고 싶은 명령어 작성 체계를 제공하기 때문에, 프로그래머들은 프로그래밍 하기 원하는<br/>
        시스템에 의존적으로 언어를 선택하기도 한다. 그러나, 그러한 시스템 의존적인 언어를 벗어나기 위해서<br/>
        여러가지 대안할 수 있는 언어들도 등장했기 때문에, 제일 많이 커버할 수 있는 언어체계를 택하여 공부하는 것이 효율이 높다.<br/>
        <br/>
        하지만, 어떤 언어라도 3-4년 정도 공부하게되면, 이 프로그래밍 언어에서 제공하는 것을 다른 언어에서는 제공하지 않는 경우는<br/>
        거의 없기 때문에, 일단 하나라도 빠삭하게 공부하는 것이 좋다.
        <br/>
        <br/>
        예) hello world 프린트하기 코드 언어별 차이<br/>
        javascript 코드
        ```javascript
        console.log("hello world")
        ```
        python 코드
        ```python
        print('hello world')
        ```
        C, C++ 코드
        ```C
        printf("hello world");
        ```
        java 코드
        ```java
        System.out.println("hello world");
        ```
        <br/>
        etc...

        <img src="https://github.com/dogfoots/schs_lect/blob/main/lecture1/dev_scheme.PNG" title="dev scheme" alt="dev scheme"></img>

    - 교육목표
        <pre>이 전체 과정을 이수한 사람은 왠만한 기업에 들어가더라도 바로 실무에 투입 가능한 수준의<br/>프로그래밍 기능인을 만드는데 있다.</pre>
        <br/>
        꼭 병행해야 하는 학과 공부 : 영어, 수학(Not 연산, 논리에 대한 부분을 말함. 특히 함수와 그래프, 확률 통계, 수체계(정수, 실수, 0과 제곱 개념))
        <br/><br/>
        프로그래밍 언어 체계상, 사실 컴퓨터의 하드웨어적인 레벨에서부터 이해하는 것이 필요하여<br/>
        Assembler나 C, C++와 같은 low-level 언어를 배우는 것이 가상 메모리 이해와<br/>
        프로그래밍 언어 이해를 깊이있게 해주지만,<br/>
        우리나라에서나 해외 트렌드에 따라서 해당 언어들의 수요가 많이 없기 때문에<br/>
        웹 개발을 중심으로 공부하도록 한다. 그리고 조금 더 시간이 주어진다면 <br/>low-level 언어들까지 학습할 기회를 만들 것.<br/>
        <br/>
        <pre>HTML, CSS, JAVASCRIPT를 먼저 학습 할 것, 그리고 python을 학습할 것(대학 대비),<br/>실무를 위해서 필요한 SQL구문도 학습해야 함<br/>좀 더 OS/하드웨어적인 진로 개척을 원한다면 C, C++까지 학습.</pre>

* 소스 형상관리
    - 소스 형상관리란
        협업에 있어서 많은 사람들과 같은 프로젝트에서 소스를 공유하고 함께 작업하는데<br/>
        이력관리 및 소스 통합이 가능하도록 하는 관리를 말함.<br/>
        이를 돕기 위해서 많이 쓰이는 형상 관리 툴들이 있는데, **SVN(SubVersioN)**과 **Git**이 있다.
    - svn
        서버의 repository(저장소)에 해당 프로젝트의 소스코드를 commit하여 올리거나, update하여 로컬 컴퓨터에<br/>
        내려받을 수 있다. check out을 통해서 서버의 프로젝트를 로컬 컴퓨터에 이관시키고<br/>
        그때부터 로컬 개발 컴퓨터에서 작업한 내용을 commit하거나 서버에 올라가있는 최신버전을 update받아서<br/>
        최신버전으로 바꿀 수 있다. 이때, 로컬에서 작업한 내용과 서버에서 업데이트 받는 내용이 충돌이 날 경우<br/>
        conflict라는 경고가 나타나고, 이를 소스 편집을 통해서 통합시킬 수 있다.
    - git
        SVN에서 발전된 형태로 서버의 repository(저장소)와 로컬 컴퓨터의 repository(저장소)가 따로 존재한다.<br/>
        이렇게 나눈 이유는, branch라는 버전 관리의 특성이 필요해졌기 때문이다.(SVN은 이러한 버전관리가 안 됨)<br/>
        따라서 로컬 개발 컴퓨터에서 작업한 내용을 먼저 로컬 repository(저장소)에 commit 시키고, 로컬 저장소에서<br/>
        커밋된 모든 내용을 최종적으로 서버의 repository에 push(commit의 개념) 시킨다.<br/>
        서버에 있는 가장 최근 업데이트 내용을 Fetch(SVN의 update 개념) 받아서 갱신할 수 있다.

* editor
    - 종류들
    - notepad plus
    - visual studio code

* web browser
    - types

* web server

* html(hypert text markup language)
* css(cascading style sheets)
* javascript

* 운영체제(operating system)


* * *
#### tasks
* google 회원가입 - 휴대폰 필요
* github 가입
* github desktop 설치
* chrome 설치
* visual studio code 설치
