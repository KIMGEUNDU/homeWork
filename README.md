# Homework
멋사 프론트엔드 스쿨 6기 과제 저장소입니다.

## mission-1 Validation, 웹 관련 용어 dl
### 💻 Html
 <br>
 
1. ***validation.html*** 마크업 순서
    1. ul.vdt-container 
    2. li.vdt__item

 Validation에 관련된 목록이라고 생각을 하여 ul 태그로 마크업했습니다.
<br> 

 2. ***term.html*** 마크업 순서
    1. article
    2. h3
    3. dl > dt + dd

홈페이지 전체를 보았을 때 독립적인 요소라고 생각이 들어 article태그로 감싸주었고 h3 로 웹관련용어라는 제목을 넣었습니다.
그 다음 웹 관련 용어에 대한 설명들은 각각 따로 dl태그로 묶어 dt 와 dd로 나눠주었습니다.

<br>
<br>

### 💻 CSS
⚒️ 참고 width, height, padding, margin, color, font-family, font-size, font-weight, line-height 는 전부 Figma 시안대로 했습니다.

#### validation.css

```
a {
  display: block;
}
```
a 요소에 display: block 을 주어 텍스트만이 아닌 전체도 클릭할 수 있도록 만들어주었습니다.
<br>

```
.vdt__item {
  background: url(../image/validation_icon2.png) no-repeat 13%/ 16px 17px #cccccc;
}
```
네모 아이콘을 배경이미지로 넣어서 위치를 조정해주었습니다.
<br>

#### term.css

```
/* W3C 이미지 */
.st__left {
  float: left;
}
```
첫 번째 이미지를 float: left를 주어 왼쪽 정렬 해주었습니다.
<br>

```
.st__right {
  float: right;
}
```
두 번째 이미지는 float: right를 주어 오른쪽 정렬 해주었습니다.

```
.webTitle {
  display: inline;
}
```
float 정렬 된 이미지들로 인해 이미지 위로 정렬되는 .webTitle을 inline 요소로 변경해주어 이미지 옆에 위치할 수 있도록 만들었습니다.

<br>
<br>

### 완성샷
<img src="https://github.com/KIMGEUNDU/homeWork/assets/126174401/3f72c7ce-7ea3-4ca3-9a75-9ea4c7a3ff7e">
<img src="https://github.com/KIMGEUNDU/homeWork/assets/126174401/e138ee2e-ffe7-4c2b-9713-ea49e145c1cd">

<br>
<br>

## mission-2 Login Form
### 💻 Html
1. 마크업 순서  
    1. 로그인 (제목)  
    2. 아이디
    3. 비밀번호
    4. 로그인버튼
    5. 회원가입 및 아이디/비밀번호 찾기  

과제 필수 조건을 맞추기 위해 위와 같이 마크업을 하였습니다.<br>
마지막 회원가입 및 아이디/비밀번호 찾기를 ul 태그로 준 이유는 회원 가입 서비스를 위한 목록이라고 생각했기 때문입니다.

<br>

🔻아래 사진 참고
<br>

<img src="https://github.com/KIMGEUNDU/homeWork/assets/126174401/c827d99b-e7a7-432e-a4e2-f9555f0ddd2d" width="500px">

<br>
<br>

### 💻 CSS
⚒️ 참고 width, height, padding, margin, color, font-family, font-size, font-weight, line-height 는 전부 Figma 시안대로 했습니다.
<br>
```
label {
  width: 56px;
  display: inline-block;
}
```
* label 태그에 width값을 주고 싶어서 display를 inline-block으로 주었습니다.
<br>

```
.loginForm {
  display: inline-block;
  box-shadow: 5px 5px 0px #AAAAAA;
}
```
* 자동으로 width값과 height 값을 잡기 위해서 inline-block 을 하였고 시안대로 그림자를 추가하였습니다.
<br>

```
/* 아이디비밀번호 래퍼 */
.loginWrapper {
  position: relative;
  border-radius: 0;
}
```
* loginBtn 요소에 position:absolute 를 주기 위해 loginWrapper를 기준점으로 잡아주었습니다.
border-bottom에 둥근 모서리가 없는 실선을 만들어주기 위해 초기값인 border-radius : 5px 을 없애기 위해 0값을 주었습니다.
<br>

```
/* 로그인 버튼 */
.loginBtn {
  cursor: pointer;
  position: absolute;
  top: 0;
  right: 0;
}
```
* 로그인 버튼에 마우스가 올라갔다는 걸 알려주기 위해서 cursor 모양을 변경하였고 기준점인 loginWrapper에서 움직이기 위해 absolute를 주어 오른쪽 위쪽에 위치하게 하였습니다.
<br>

```
/* 회원가입/아이디비밀번호찾기 */
.memberService {
  display: flow-root;
}
```
* 밑에 오게 될 li.memberItem 요소에 float를 주기 위해 li.memberItem의 부모 요소를 정해주어 기준점을 잡아주었습니다.
<br>

```
/* 회원가입 */
.memberItem:first-child {
  float: left;
}

/* 아이디비밀번호찾기 */
.memberItem:last-child {
  float: right;
}
```
* 회원가입 요소는 왼쪽으로 아이디비밀번호찾기 요소는 오른쪽으로 위치를 정해주었습니다.
<br>
<br>

### 완성샷

![image](https://github.com/KIMGEUNDU/homeWork/assets/126174401/bfc859f5-6bda-4fa5-9bc3-d7c5fa52c68e)
