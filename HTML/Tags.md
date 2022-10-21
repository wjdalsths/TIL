# 웹페이지 기본 태그

## 1. 문서 형식 정의 tag

---

문서 형식 정의(Document Type Definition, DTD) 태그는 출력할 웹 페이지의 형식을 브라우저에게 전달한다. 문서의 최상위에 위치해야 하며 대소문자를 구별하지 않는다.

### `HTML5`

```html
<!DOCTYPE html>
```

## 2. html tag

---

html 태그는 모든 HTML 요소의 부모 요소이며 웹페이지에 단 하나만 존재한다. 즉, 모든 요소는 html 요소의 자식 요소이며 html 요소 내부에 기술해야 한다. 단 <!DOCTYPE>는 예외이다.

```html
<!DOCTYPE html>
<html lang="ko">
  <!-- lang 어트리뷰트 -->
  <head>
    <meta charset="utf-8" />
    <title>문서 제목</title>
  </head>
  <body>
    화면에 표시할 모든 콘텐츠는 이곳에 기술한다.
  </body>
</html>
```

## 3. head tag

---

head 요소는 메타데이터를 포함하기 위한 요소이며 웹페이지에 단 하나만 존재한다. 메타데이터는 HTML 문서의 title, style, link, script에 대한 데이터로 화면에 표시되지 않는다.

head 요소에는 메타데이터 이외의 화면에 표시되는 일체의 요소를 포함시킬 수 없다.

## 3.1 title tag

title 요소는 문서의 제목을 정의한다. 정의된 제목은 브라우저의 탭에 표시된다.

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8" />
    <title>문서 제목</title>
  </head>
  <body>
    Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
    tempor incididunt ut labore et dolore magna aliqua.
  </body>
</html>
```

## 3.2 style tag

style 요소에는 HTML 문서를 위한 style 정보를 정의한다.

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8" />
    <title>문서 제목</title>
    <style>
      body {
        background-color: yellow;
        color: blue;
      }
    </style>
  </head>
  <body>
    Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
    tempor incididunt ut labore et dolore magna aliqua.
  </body>
</html>
```

## 3.3 link tag

link 요소에는 외부 리소스와의 연계 정보를 정의한다.

```html
<html>
  <head>
    <meta charset="utf-8" />
    <title>문서 제목</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body></body>
</html>
```

## 3.4 script tag

script 요소에는 JavaScript를 정의한다.<br>
src 어트리뷰트를 사용하면 외부 JavaScript 파일을 로드할 수 있다.

```html
<html>
  <head>
    <meta charset="utf-8" />
    <script>
      document.addEventListener("click", function () {
        alert("Clicked!");
      });
    </script>
  </head>
  <body></body>
</html>
```

## 3.5 meta tag
