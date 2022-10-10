# HTML: Hyper Text Markup Language

HTML은 프로그래밍 언어가 아니라 마크업 정보를 표현하는 마크업 언어이다. HTML은 요소(elements)로 구성되어 있으며 각 컨텐츠의 여러 부분들을 감싸고 마크업 한다.

---

HTML 파일의 기본 템플릿

```html
<!DOCTYPE html>
<html>
  <head>
    --
    <meta charset="UTF-8" />
    <title>Document</title>
  </head>
  <body>
    --
  </body>
</html>
```

---

## HTML 기본구조

### `Element(요소)`

- html 에서 개별적인 역할을 하는 태그를 말한다.

```html
<h1></h1>
```

### `Tag(태그)`

<img src="https://s3.us-west-2.amazonaws.com/secure.notion-static.com/64956634-fc86-4d90-a0c5-68ae8eae7531/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20221010%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20221010T055748Z&X-Amz-Expires=86400&X-Amz-Signature=a66cfdc7737422da4be114e8771f25ea6a57d4eaf6b34a2bfb8743e3fedd2d6d&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22&x-id=GetObject" width="600" height="160"/>

- 객체를 만들때 사용한다.
- 시작 태그(opening tag)를 시작으로 끝태그(closing tag)로 끝나는 모든 객체를 태그라고 한다.

### `Attribute(속성)`

<img src="https://velog.velcdn.com/images%2Fheartane%2Fpost%2Fc44ec593-1977-407b-aa06-8abdc6520c40%2FScreen%20Shot%202021-06-30%20at%209.20.03%20PM.png" width="600px" height="">

- 태그에 추가로 정보를 제공하거나 태그의 동작이나 표현을 제어하는 설정값
- 여러개의 속성을 사요할 때 공백(뛰어쓰기)으로 구분
- Global Attribute:
  Id / class / hidden / lang / style / tabindex / title

### `Content(내용)`

- 시작태그와 끝내그 사이의 내용

```html
<div>|content|</div>
```

---

## HTML 문서의 구조

1. `<!DOCTYPE html>` 유효한 문서 형식을 나타내는 짧은 문장이다.
2. `<html></html>` 이 요소는 전체 페이지의 콘텐츠를 포함한다.
3. `<meta charset="utf-8">` 이 요소는 HTML문서의 문자 인코딩 설정을 UTF-8로 지정하는 것이다.
4. `<head></head>` 이 요소는 보이지 않는 모든 HTML페이지의 내용을 담고 있다(문서 정보(메타데이터)).
5. `<body></body>` 이 요소는 페이지에 표시되는 모든 콘텐츠를 포함한다.
6. `<title></title>` 이 요소는 페이지가 로드되는 브라우저의 탭에 표시되는 제목을 설정한다.
