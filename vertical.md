방법 1 - padding 속성 이용하기
바깥쪽 요소에 padding 속성을 추가해서 세로 정렬을 가운데로 할 수 있습니다.
<pre><code>
<!doctype html>
<html lang="ko">
  <head>
    <meta charset="utf-8">
    <title>CSS</title>
    <style>
      body {
        box-sizing: border-box;
        font-family: Consolas, monospace;
      }
      .jb-wrap {
        border: 1px solid #444444;
        padding: 100px 0px;
      }
      h1 {
        padding: 20px 0px;
        background-color: #444444;
        text-align: center;
        color: #ffffff;
      }
    </style>
  </head>
  <body>
    <div class="jb-wrap">
      <h1>Lorem Ipsum Dolor</h1>
    </div>
  </body>
</html>
</code></pre>


방법 2 - margin 속성 이용하기
안쪽 요소에 margin 속성을 추가해서 세로 정렬을 가운데로 할 수 있습니다.
<pre><code>
<!doctype html>
<html lang="ko">
  <head>
    <meta charset="utf-8">
    <title>CSS</title>
    <style>
      body {
        box-sizing: border-box;
        font-family: Consolas, monospace;
      }
      .jb-wrap {
        border: 1px solid #444444;
      }
      h1 {
        margin: 100px 0px;
        padding: 20px 0px;
        background-color: #444444;
        text-align: center;
        color: #ffffff;
      }
    </style>
  </head>
  <body>
    <div class="jb-wrap">
      <h1>Lorem Ipsum Dolor</h1>
    </div>
  </body>
</html>
</code></pre>
 
 
 
방법 3 - 표(table)처럼 만들기
표처럼 만들고 세로 가운데 정렬을 가운데로 할 수 있습니다. 높이를 정하기 쉽다는 장점이 있으나 코드가 많아진다는 단점이 있습니다.
<pre><code>
<!doctype html>
<html lang="ko">
  <head>
    <meta charset="utf-8">
    <title>CSS</title>
    <style>
      body {
        box-sizing: border-box;
        font-family: Consolas, monospace;
      }
      .jb-table {
        display: table;
        width: 100%;
        height: 280px;
        border: 1px solid #444444;
      }
      .jb-table-row {
        display: table-row;
      }
      .jb-table-cell {
        display: table-cell;
        vertical-align: middle;
      }
      h1 {
        padding: 20px 0px;
        background-color: #444444;
        text-align: center;
        color: #ffffff;
      }
    </style>
  </head>
  <body>
    <div class="jb-table">
      <div class="jb-table-row">
        <div class="jb-table-cell">
          <h1>Lorem Ipsum Dolor</h1>
        </div>
      </div>
    </div>
  </body>
</html>
</code></pre>



방법 4 - Flex 이용하기
CSS3의 flex를 이용하면 쉽게 세로 가운데 정렬을 구현할 수 있습니다. 하지만 IE 11부터 지원한다는 문제가 있습니다.
<pre><code>
<!doctype html>
<html lang="ko">
  <head>
    <meta charset="utf-8">
    <title>CSS</title>
    <style>
      body {
        box-sizing: border-box;
        font-family: Consolas, monospace;
      }
      .jb-wrap {
        height: 280px;
        display: flex;
        align-items: center;
        border: 1px solid #444444;
      }
      h1 {
        width: 100%;
        padding: 20px 0px;
        background-color: #444444;
        text-align: center;
        color: #ffffff;
      }
    </style>
  </head>
  <body>
    <div class="jb-wrap">
      <h1>Lorem Ipsum Dolor</h1>
    </div>
  </body>
</html>
</code></pre>




출처 : https://www.codingfactory.net/10835
