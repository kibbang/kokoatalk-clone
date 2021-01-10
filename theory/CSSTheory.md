# CSS

# CSS를 HTML페이지에 추가하는가

-> 같은 페이지에 코드를 두는것
-> 분리시켜두는것

같은 페이지에 코드를 두는것

<style>사용 (<head> 안에 있어야 함)

2. 분리시켜두는것
파일을 만든후 <link>로 연결
<link href="~~.css" rel="stylesheet">

CSS코드의 작성 규칙

selector(가르키는 대상) {
    ~~~~~
}

속성: 값;

태그를 지정하고 속성을 쓰기만 하면 됨


BOX

옆에 다른 요소가 못오는것을 block
다른 요소가 올 수 있는것을 inline이라 함

block이 아닌것 span, a, img

그러면 block을 inline으로 inline을 block으로 바꿀 수 있는가? -> yes
display 속성을 이용한다.

* display: inline은 높이와 너비가 적용되지 않는다.

margin: box의 border(경계)로 부터 바깥에 있는 공간

margin: 10px면 상하좌우 다 10
margin: 10px 20px면 상하 10 좌우 20
margin: 10px 20px 30px 40px면 상 10 우 20 하 30 좌 40 (시계방향순)


* collapsing margin: 두 box의 경계가 같을때 두 box는 하나로 취급되는 현상
상,하로만 일어남

그래서 나타난 것이 padding

padding: box의 border(경계)로 부터 안쪽에 있는 공간

id 지정법: #id

border: box의 경계
거의 1가지만 씀 solid
border: size, style, color

전체 = *

inline은 margin 을 좌 우만 가질 수 있음
다 가지게 하려면 block으로 바꿔야 함

class: 겹쳐서 사용할 수 있음 한 element에 여러 개 가질 수 있음
.class{

}

inline-block
block을 inline으로 가질 수 있음
하지만 별로다(문제가 많음, 정해진 형식이 없음)

inline-block의 문제점을 해결하기 위해 나온것이 flex

flexbox의 자식 element에는 아무것도 적지 말아야 한다.
부모 element에 적용함

flex의 옵션
1. justify-content(수평)
2. align-item (수직)

vh -> viewpoint height

flex-direction 수평 수직 설정

position: 아주 조금씩 움직이고 싶을때
fixed: 고정
relative: 처음 위치한 곳으로부터(기준으로) 수정하는 것
absolute: 가장 가까운 relative 부모를 기준으로 이동시켜줌

pseudo-selector : 좀 더 세부적으로 선택할 수 있게 해줌
ex) div:last-child {
    color: ~~~~
}
nth-child(2) 두번째 것
짝수는 nth-child(even)
홀수는 nth-child(odd)

div > span
div안(바로 밑)에 span 속성을 가르킴

형제에게 주는 방법(바로 뒤)
p + span

바로 뒤가 아닌 경우
p ~ span

pseudo-selector로 선택
state
action: click
hover: mouse가 위에 있을 때
focus: 키보드로 클릭했을 때
focus-within: 부모에 적용되는 focus


pseudo element
실제 존재하는 element는 아니지만, 특정 요소의 부분을 꾸미게 해줌.
ex)
::placeholder
::selection
::first-letter

color= rgb로 많이 씀
rgba = rgb에 투명도 (alpha)를 추가한 것


transition

어떤 상태변화를 애니매이션으로 만드는 것
state 속성이 없는 쪽에 붙어야 함(이게 제일 중요)

transition: 변화시킬 요소, 걸릴 시간
ex) transition: background-color 10s
변화 하는 모든것에 하고 싶으면
transition: all

ease-in function
애니메이션이 어떻게 변하는가

transform
상태변형
다른 형제를 변형시키지는 않는다

애니메이션을 계속 가지고 싶다면?
@keyframes animation name {
    from {
        ~~~~
    } to {
        ~~~~
    }
}

후  css 속성에 animation: animation name 5s ease-in-out 이런식 여기에 infinite를 추가 하면 무한으로 작동

꼭 from to가 아니라 %로 나누어 할 수도 있음


media query

@media screen and (max-width = 600px)
600px 보다 작을때 적용

orientation: landscape 가로모드
              portrait 세로모드
