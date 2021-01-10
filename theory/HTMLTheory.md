# HTML tag

# HTML tag는 엄청 많음 그러니 검색해서 사용하는게 좋음 (覚える必要はない)

→ 　 HTML MDN

# <ul> -> unordered list 　걍 점이 표시됨 丸点が表示される

# <ol> -> ordered list 숫자가 표시됨 数字が表示される

# <li> -> list item

# <a> -> anchor 링크태그 リンクタグ　 attribute가 필요함 attribute が必要

-> href: hyperlink reference or HTTP reference
-> ex) <a href="~~~~~~">~~~</a>
-> a 태그의 다른 attribute: target
-> target은 default가 　\_self 自分
-> \_blank는 다른 탭에서 열림 新しブラウザ

# <img>

-> 닫는 태그가 없음 self-closing tag
-> attribute는 src
-> ex) <img src="~~~~~~~~~~~~~~~~~~" />
-> 데스크톱에 있는 걸 올릴때는 경로를 잘 적어줘야 함

# <meta>

-> self-closing tag
-> 부가정보 (subInfomation)
title, base, link, style

<meta property og:image>는 메신저 대화방에 공유될때 보이는 이미지

<meta charset>은 중요함!!! 大事
브라우저에게 text를 어떻게 그려달라 하는걸 알려줌

# HTML 문서의 구조

화면상에 보여질 것은 전부 <body>태그에 넣는다.
画面上に見える物は全部<body>タグに入れる。

1. <!DOCTYPE html>
2. <html></html>
3. <head></head>, <body></body>
   -> 브라우저에게 사이트가 어떻게 보여지는가 알려주는게 head의 역할
4. <meta> 부가정보

<form></form>
-> 모든 정보를 넣는다.
<input> 입력폼
placeholder <input>의 속성

<tagname attrname="attribute">~~~~~~~~~~~~~~~</tagname>

<label>의 for와 <input>의 id는 같아야한다.
<label for="aaa"><input id="aaa">

id는 body안에 어떤 태그에도 사용할 수 있는 속성(고유 식별자 이기 때문)
1개당 1개의 id를 가진다.

# <div> (division)

-> box역할

# Sementic Tags(의미 없는 태그)

<header></header> 이거는 <head>랑 다름 body안에 있는거임 주의!
<main>
<footer>
<span> 짧은 텍스트 옆에 다른 요소가 올 수 있다.
<p> 단락
