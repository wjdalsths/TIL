# CSS 크기 단위

css 크기 단위에는 대표적으로 px,%,em,rem,viewport 등이 있다.

- `절대값`: px
- `상대값`: %,em,rem,viewport

---

1.  ## px

    px은 픽셀(화소) 단위이다. 1px은 화소 1개의 크기를 의미한다.

    ### 단점

    - 픽셀은 해상도에 따라 상대적인 크기를 갖는다.
    - 그로인해 픽셀의 크기는 제각각이다.

---

2.  ## %

    %는 백분률 단위의 상대 단위이다. 요소에 지정된 사이즈에 상대적인 사이즈를 설정한다.

    ```html
    <style>
      body {
        font-size: 14px;
      }
      div {
        font-size: 120%;
      }
    </style>
    <body>
      <div>fontsize: 14px * 120% = 16.8px</div>
    </body>
    ```

---

3.  ## em

    em은 배수 단위로 상대 단위이다. 요소에 지정된 사이즈에 상대적인 사이즈를 설정한다.

    ```html
    <style>
      body {
        font-size: 14px;
      }
      div {
        font-size: 1.2em;
      }
    </style>
    <body>
      <div>fontsize: 1.2em -> 14px * 1.2 = 16.8px</div>
    </body>
    ```

    중첩된 자식 요소에 em을 지정하면 모든 자식 요소의 사이즈에 영향을 미치기 때문에 주의해야 한다.

    ```html
    <style>
      body {
        font-size: 14px;
      }
      div {
        font-size: 1.2em;
      }
    </style>

    <body>
      <div class="box1">
        Font size: 1.2em ⇒ 14px * 1.2 = 16.8px
        <div class="box2">
          Font size: 1.2em ⇒ 16.8px * 1.2 = 20.16px
          <div class="box3">Font size: 1.2em ⇒ 20.16px * 1.2 = 24.192px</div>
        </div>
      </div>
    </body>
    ```

---

4.  ## rem('r'oot + em)

    rem은 최상위 요소(html)의 사이즈를 기준으로 삼는다.

    ```html
    <style>
      html {
        font-size: 14px;
        /* font-size 미지정 시에는 16px */
      }
      div {
        font-size: 1.2rem;
        font-weight: bold;
        padding: 2em;
        text-align: center;
      }
    </style>

    <body>
      <div class="box1">
        Font size: 1.2rem ⇒ 14px * 1.2 = 16.8px
        <div class="box2">
          Font size: 1.2rem ⇒ 14px * 1.2 = 16.8px
          <div class="box3">Font size: 1.2rem ⇒ 14px * 1.2 = 16.8px</div>
        </div>
      </div>
    </body>
    ```

    ### 장점

    - 사용자가 브라우저의 기본 폰트 크기를 변경하더라도 이에 따라 웹사이트의 레이아웃을 적절히 조정할 수 있다는 장점이 있다.

---

5.  ## Viewport 단위(vh, vw, vmin, vmax)

    Viewport 단위는 상대적인 단위로 viewport를 기준으로 한 상대적 사이즈를 의미한다.

    ###### \* viewport는 웹페이지가 사용자에게 보여지는 영역을 말합니다.

    예)

    `width: 50vw` : viewport 너비의 50%

    ### 종류

    <table border="1">
        <tr>
            <td>단위</td>
            <td>설명</td>
        </tr>
        <tr>
            <td>vw</td>
            <td>viewport 너비의 %</td>
        </tr>
        <tr>
            <td>vh</td>
            <td>viewport 높이의 %</td>
        </tr>
        <tr>
            <td>vmin</td>
            <td>viewport 너비 또는 높이 중 작은 쪽의 %</td>
        </tr>
        <tr>
            <td>vmax</td>
            <td>viewport 너비 또는 높이 중 큰 쪽의 %</td>
        </tr>
    </table>
