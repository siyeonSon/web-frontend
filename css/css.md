## CSS
- HTML이 정보 전달에 전념하기 위해서, 디자인과 관련된 새로운 언어의 등장
- HTML만으로 디자인하는 것보다, CSS를 활용하는 것이 더욱 효율적임
  - 예: 태그마다 디자인을 삽입하는 것이 아닌, 해당 태그에 대한 디자인을 일괄적으로 삽입할 수 있음

### `<style>` 사용
```css
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
```
<li><a href="2.html" style="color:red; text-decoration:underline;">CSS</a></li>
```

<br>

### 선택자(selector)
#### 태그 선택자 ( { })
- `a { color: black }`

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
