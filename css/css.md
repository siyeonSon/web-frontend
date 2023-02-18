## CSS
- HTML이 정보 전달에 전념하기 위해서, 디자인과 관련된 새로운 언어의 등장
- HTML만으로 디자인하는 것보다, CSS를 활용하는 것이 더욱 효율적임
  - 예: 태그마다 디자인을 삽입하는 것이 아닌, 해당 태그에 대한 디자인을 일괄적으로 삽입할 수 있음

### `<style>` 사용
```html
<head>
  <style>
    a {
      color: black;
      text-decoration: none;
    }
  </style>
</head>
```
- `a { }` : 태그 선택자(selector)
- `color:black;` : 선언(declaration) / 효과
- `color` : 속성(property)
- `black` : 값(value)

<br>

### `style` 속성 사용
```html
<li><a href="2.html" style="color:red; text-decoration:underline;">CSS</a></li>
```

<br>

### 선택자(selector)
#### 태그 선택자 ( { })
- `a { color: black; }`

#### class 선택자 (. { })
- HTML에 class 지정
  - `<li><a href="1.html" class="saw">HTML</a></li>`
- CSS 속성 부여
  - `.saw { color: grey; }`

#### id 선택자 (# { })
- id 값은 한번만 등장해야 함
- HTML에 id 지정
  - `<li><a href="2.html" class="saw" id="active">CSS</a></li>`
- CSS 속성 부여
  - `#active { color: red; }`

<br>

### 박스 모델
- block level element: 화면 전체를 차지하는 태그
  - 예: `<h1>`
- inline level element: 자기 크기만큼을 차지하는 태그
  - 예: `<a>`

- `display: inline` `display: block` `display: none`  등과 같은 CSS 속성을 통해 박스 모델 수정 가능

#### 코드 양 줄이기
```css
/** 기존 **/
h1 {
  border-width: 5px;
  border-color: red;
  border-style: solid;
}
a {
  border-width: 5px;
  border-color: red;
  border-style: solid;
}

/** 줄이기 **/
h1, a {
  border-width: 5px;
  border-color: red;
  border-style: solid;
}

/** 더 줄이기**/
h1, a {
  border: 5px solid red;
}
```

<br>

### 여백
```css
h1 {
    border: 5px solid red;
    padding: 20px;
    margin: 0;
    width: 100px;
}
```

- content - padding - border - margin

<img src="https://static.javatpoint.com/csspages/images/margin-padding.png">

<br>

### 그리드
- 참고
  - 디자인을 위한 태그
    - `<div>` : block level element
    - `<span>`: inline level element

- grid 사용
```html
<head>
  <style>
      #grid {
          border: 5px solid pink;
          display: grid;
          grid-template-columns: 150px 1fr;  /* NAVIGATION은 150px 크기를, ARTICLE은 나머지 크기를 가짐 */
      }
      div {
          border: 5px solid gray;
      }
  </style>
</head>
<body>
    <div id="grid">
        <div>NAVIGATION</div>
        <div>ARTICLE</div>
    </div>
</body>
```

![image](https://user-images.githubusercontent.com/87802191/219864751-597a8f96-5481-40ca-ab87-b71acfcedbee.png)

- `1fr` : CSS 화면 단위
  - `1fr 1fr` : 1:1 비율
  - `2fr 1fr` : 2:1 비율