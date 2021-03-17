# practice
My first practice git-hub


콘솔을 통한 컴파일
[Sass를 통한 컴파일]
: Sass는 단순하게 컴파일을 위해서 꼭 필요한 프로그램 이다. 다양한 Sass 컴파일러 들은 이 Sass 프로그램 의존적 이다.

> Sass 프로그램 설치

- 윈도우
Sass는 ruby 가 설치 되어 있어야 한다. (윈도우용 ruby : http://rubyinstaller.org/)
ruby 설치 후 Command 창으로 들어가서 다음을 치면 sass가 설치된다.<br>
    gem install sass
<br><br>

- 맥
맥은 기본적 으로 ruby가 설치되어 있기 때문에, 별다른 과정 없이 터미널 에서 설치를 진행하면 된다.<br>
    gem install sass
<br><br>

<br><br>
> 컴파일 하기

- 한개의 파일을 컴파일 하는 방법은<br>
    sass input.scss output.css

앞이 컴파일을 하는 scss 파일이고, 뒤에 css 파일명이 컴파일 후 생성되는 파일 이름이다.
이렇게 하면 output.css 파일과 output.map 파일이 생기는데, output.css는 컴파일이 진행된 파일이고, map 파일은 scss 와 css가 어떻게 연결 되어 있는지에 대한 정보 파일 정도로 이해 하면 된다.
