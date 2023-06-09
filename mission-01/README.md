# mission-1 Validation, 웹 관련 용어 dl
## 💻 Html
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

## 💻 CSS
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

## 완성샷
<img src="https://github.com/KIMGEUNDU/homeWork/assets/126174401/3f72c7ce-7ea3-4ca3-9a75-9ea4c7a3ff7e">
<img src="https://github.com/KIMGEUNDU/homeWork/assets/126174401/e138ee2e-ffe7-4c2b-9713-ea49e145c1cd">

<br>
<br>