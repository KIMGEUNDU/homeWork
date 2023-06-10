# mission-2 Login Form
## 💻 Html
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

## 💻 CSS
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

## 완성샷

<img src="https://github.com/KIMGEUNDU/homeWork/assets/126174401/bfc859f5-6bda-4fa5-9bc3-d7c5fa52c68e">
