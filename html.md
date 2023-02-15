# HTML 기본 문법
## HTML
- Hypertext Markup Language
- HyperText(웹 페이지에서 다른 페이지로 이동할 수 있도록 하는 것) 기능을 가진 문서를 만드는 언어

<br>

## 태그
- 예: <strong>Hypertext Markup Language(HTML)</strong> is the standard markup language for <strong>creating <u>web</u> pages</strong> and web applications.
  - `<strong>Hypertext Markup Language(HTML)</strong> is the standard markup language for <strong>creating <u>web</u> pages</strong> and web applications.`
    - `<strong>` : 굵게
    - `<u>` : 밑줄

        
### 줄바꿈
- `<br>`
  - 줄바꿈
  - 원하는 만큼 간격을 줄 수 있음
- `<p> </p>`
  - 단락
  - 단락과 단락의 간격이 고정되어 있기 때문에 시각적으로 자유도가 떨어짐

- CSS를 이용하면 p태그의 한계를 극복할 수 있음
  - `<p style="margin-top:45px;">` : p 태그의 위쪽에 45px 만큼의 여백(margin)이 생김

<br>

## 속성
- 예: `<img src="https://s3-ap-northeast-2.amazonaws.com/opentutorials-user-file/module/3135/7648.png" width="100%">`
  - `<img>` 태그와 `src`, `width` 속성

<br>

## 목록
- <strong>unordered</strong> list
```html
<ul>
  <li>HTML</li>
  <li>CSS</li>
  <li>JavaScript</li>
</ul>
```
<ul>
  <li>HTML</li>
  <li>CSS</li>
  <li>JavaScript</li>
</ul>

<br>

- <strong>ordered</strong> list
```html
<ol>
  <li>HTML</li>
  <li>CSS</li>
  <li>JavaScript</li>
</ol>
```
<ol>
  <li>HTML</li>
  <li>CSS</li>
  <li>JavaScript</li>
</ol>

<br>

## 문서의 기본 구조
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>
</head>
<body>
  
</body>
</html>
```

- `<!DOCTYPE html>` : 문서가 HTML로 만들어졌음을 나타냄
- `<html>` 태그 아래에 `<head>`, `<body>` 태그 존재
  - `<html>` : 문서에서 다룰 언어 지정
  - `<head>` : 문서의 메타데이터(웹페이지의 요약)
  - `<body>` : 콘텐츠 작성

  <br>

## 링크
- 예 : `<a href="index.html">`
- <a href="https://web-n.github.io/web1_html_internet/">결과물
- <a href = "https://github.com/web-n/web1_html_internet">소스코드
```html
<!doctype html>
<html>
<head>
  <title>WEB1 - html</title>
  <meta charset="utf-8">
</head>
<body>
  <h1><a href="index.html">WEB</a></h1>
  <ol>
    <li><a href="1.html">HTML</a></li>
    <li><a href="2.html">CSS</a></li>
    <li><a href="3.html">JavaScript</a></li>
  </ol>
  <h2>HTML</h2>
  <p><a href="https://www.w3.org/TR/html5/" target="_blank" title="html5 speicification">Hypertext Markup Language (HTML)</a> is the standard markup language for <strong>creating <u>web</u> pages</strong> and web applications.Web browsers receive HTML documents from a web server or from local storage and render them into multimedia web pages. HTML describes the structure of a web page semantically and originally included cues for the appearance of the document.
  </p><p style="margin-top:45px;">HTML elements are the building blocks of HTML pages. With HTML constructs, images and other objects, such as interactive forms, may be embedded into the rendered page. It provides a means to create structured documents by denoting structural semantics for text such as headings, paragraphs, lists, links, quotes and other items. HTML elements are delineated by tags, written using angle brackets.
  </p>
</body>
</html>
```