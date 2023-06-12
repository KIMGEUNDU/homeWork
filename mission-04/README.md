# mission-3 Transition
## 💻 Html
1. 마크업 순서  
    1. section 
    2. h2.relatedSiteTitle
    3. ul.siteLinkWrapper
    4. li
    5. a.siteLink


```section```으로 묶고 마크업을 시작했습니다.  
제목을 h2로 정하였고 링크들은 ul태그로 묶었습니다.  
제목에 '사이트'에만 다른 색을 지정하기 위해 ```span```태그로 묶어놨습니다.


<br>

🔻아래 사진 참고
<br>
<img src="https://github.com/KIMGEUNDU/homeWork/assets/126174401/57e1774a-7563-4e99-a6b5-9293a7242cae" width="500px">


<br>
<br>

## 💻 CSS
⚒️ 참고 width, height, padding, margin, color, font-family, font-size, font-weight, line-height 는 전부 Figma 시안대로 했습니다.
<br>
<br>

```
/* 링크 래퍼 */
.siteLinkWrapper {
  overflow: hidden;
  transition-property: height, padding-top;
  transition-duration: 0.3s;
  transition-delay: 0s, 0.2s;
  height: 29px;
  padding-top: 0;
}
```
제로베이스 문구만 처음에 보였으면 좋겠어서 제로베이스 폰트 높이만큼 height를 설정하고 overflow: hidden 을 설정하였습니다.
그 뒤로 마우스 올리는 효과를 집어넣은 후 다시 돌아올 때 부드럽게 돌아왔으면 좋겠어서 height와 padding-top 을 기본값으로 맞춰주었습니다.

<br>
<br>

```
/* hover 이벤트 */
.siteLinkWrapper:hover {
  transition-property: height, padding-top;
  transition-duration: 0.6s;
  transition-delay: 0s, 0.4s;
  transition-timing-function: linear;
  height: 175px;
  padding-top: 10px;
}
```
마우스를 올렸을 때 ul영역이 늘어나면서 숨겨져있던 리스트를 보여주고 싶어서 transition-property에 height를 추가했습니다.
그리고 리스트가 다 펼쳐지고 안에 있는 링크들이 한번 더 내려왔으면 좋겠어서 padding-top 속성도 추가했습니다.

<br>
<br>

## 완성샷

<br>
<br>
<img src="https://github.com/KIMGEUNDU/homeWork/assets/126174401/b6a39c14-a4dc-4ce9-8f42-05275ea6c453">
