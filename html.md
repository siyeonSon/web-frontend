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