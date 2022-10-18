# Select(선택자)

CSS를 적용시킬 HTML의 요소를 정의한다.

## 종류

1. ### 기본선택자

<table border="1">
<tr>
   <th>이름</th>
   <th>구문</th>
   <th>설명</th>
</td>
<tr>
   <td>전체 선택자</td> 
   <td>*{style properties}</td> 
   <td>모든 형태의 모든 요소를 선택한다.</td>
</tr>
<tr>
   <td>태그 선택자</td> 
   <td>태그 { style properties }</td> 
   <td>해당 태그의 모든 요소를 선택한다.</td>
</tr>
<tr>
   <td>클래스 선택자</td> 
   <td>.클래스이름 { style properties }</td> 
   <td>해당 클래스의 모든 요소를 선택한다.</td>
</tr>
<tr>
   <td>ID 선택자</td> 
   <td>#아이디이름 { style properties }</td> 
   <td>해당 아이디의 모든 요소를 선택한다.</td>
</tr>
<tr>
   <td>속성 선택자</td> 
   <td>태그[속성이름="속성값"] { style properties } 
      
   </td> 
   <td>특정 속성이나 특정 속성값을 가지고 있는 요소를 선택한다.</td>
</tr>
<tr>
   <td>그룹 선택자</td> 
   <td>태그 , 태그 { style properties }</td> 
   <td>선택자 목록(,)은 일치하는 모든 요소를 선택한다.</td>
</tr>

</table>

2. ### 결합자

<table border="1">

<tr>
   <td>자손 결합자</td> 
   <td>선택자1 선택자2 { ... }</td> 
   <td>선택자1의 모든 하위 요소 중 선택자2를 선택한다.</td>
</tr>
<tr>
   <td>자식 결합자</td> 
   <td>선택자1 > 선택자 2 { style properties }</td> 
   <td>선택자1의 바로 밑의 자식 중 선택자2를 선택한다.</td>
</tr>
<tr>
   <td>일반 형제 결합자</td> 
   <td>선택자1 ~ 선택자 2 { style properties }</td> 
   <td>선택자1의 형제 중 자신보다 다음에 오는 모든 선택자2를 선택한다.</td>
</tr>
<tr>
   <td>인접 형제 결합자</td> 
   <td>선택자1 + 선택자 2 { style properties }</td> 
   <td>선택자1의 형제 중 바로 다음에 오는 선택자1 하나를 선택한다.</td>
</tr>

</table>

3. ### 가상 클래스
<table border="1">

- 구조 선택자
<tr>
   <th>구문</th>
   <th>설명</th>
</td>
<tr>
   <td>:first-child</td>
   <td>형제 중 첫 번째로 오는 요소를 선택한다.</td>
</tr>
<tr>
   <td>:last-child</td>
   <td>형제 중 마지막으로 오는 요소를 선택한다.</td>
</tr>
<tr>
   <td>:nth-child(수열)</td>
   <td>형제 중 (수열) 번째에 있는 요소를 선택한다.</td>
</tr>
<tr>
   <td>:nth-last-child(수열)</td>
   <td>형제 중 뒤에서(수열) 번째에 있는 요소를 선택한다.</td>
</tr>
</tr>
<tr>
   <td>:nth-of-type(수열)</td>
   <td>태그별로 형제 중(수열) 번째에 있는 요소를 선택한다. 태그 이외 다른 선택자에는 반응하지 않는다.</td>
</tr>

</table>

- 반응 선택자

<table border="1">
<tr>
   <td>:active</td>
   <td>클릭하고 있는 요소를 선택한다.</td>
</tr>
<tr>
   <td>:hover</td>
   <td>커서가 올라와 있는 요소를 선택한다.</td>
</tr>

<table>

- 상태 선택자

<table border="1">
<tr>
   <td>:checked</td>
   <td>체크되어 있는 input 체크박스, 라디오 버튼이나 드롭다운 메뉴의 선택되어 있는 선택지(option)를 선택한다.</td>
</tr>
<tr>
   <td>:focus</td>
   <td>현재 입력하고 있는, 즉 커서가 깜박이고 있는 input 요소를 선택한다.</td>
</tr>
<tr>
   <td>:enabled</td>
   <td>활성화되어 있는, 즉 내용을 수정할 수 있는 input 요소를 선택한다.</td>
</tr>
<tr>
   <td>:disabled</td>
   <td>비활성화되어 있는, 즉 내용을 수정할 수 없는 input 요소를 선택한다.</td>
</tr>
<table>

- 링크 선택자

<table border="1">
<tr>
   <td>:link</td>
   <td>href 속성이 명시된 a 요소를 선택한다.</td>
</tr>
<tr>
   <td>:visited</td>
   <td>방문했던 링크가 걸린 a 요소를 선택한다.</td>
</tr>
<table>

- 부정 선택자

<table border="1">
<tr>
   <td>:not(선택자)</td>
   <td>해당 선택자에 해당하지 않는 요소들을 선택한다.</td>
</tr>
<table>

- 가상 요소

<table border="1">
<tr>
   <td>::first-letter</td>
   <td>첫 번째 글자를 선택한다. ::before의 영향을 받는다. </td>
</tr>
<tr>
   <td>::first-line</td>
   <td>첫 번째 줄을 선택한다. </td>
</tr>
<tr>
   <td>::before</td>
   <td>태그 앞에 위치하는 공간을 선택한다. CSS 속성 'content'를 이용하여 이 공간에 추가로 내용을 입력할 수 있다. </td>
</tr>
<tr>
   <td>::fafter</td>
   <td>태그 뒤에 위치하는 공간을 선택한다. ::before와 같이 'content'를 이용하여 이 공간에 추가로 내용을 입력할 수 있다. </td>
</tr>
<tr>
   <td>::selection</td>
   <td>드래그한 글자를 선택한다. </td>
</tr>
<table>

---

## 선택자 우선순위

1. !important (속성: 적용 값!important)
   <br>⬇
2. 인라인 스타일 (style="")
   <br>⬇
3. ID 선택자 (#아이디이름)
   <br>⬇
4. CLASS 선택자 (.클래스이름)
   <br>⬇
5. 태그 선택자 (tag)
   <br>⬇
6. 전체 선택자 (\*)
