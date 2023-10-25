<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <header id="header">
    <div class="header-title">
      <h1>早稲田大学特撮評議会 早稲田祭特設サイト</h1>
      <h1>俳優 佐藤太輔の世界</h1>
    </div>
    <div class="hamburger-menu">
      <input type="checkbox" id="menu-btn-check" />
      <label for="menu-btn-check" class="menu-btn"><span></span></label>
      <!--ここからメニュー-->
      <div class="menu-content">
        <ul>
          <li><a href="index.html#about-container">About</a></li>
          <li><a href="index.html#plofile">Plofile</a></li>
          <li><a href="index.html#ticket">Ticket</a></li>
          <li><a href="index.html#sokubai">Contents</a></li>
        </ul>
      </div>
    </div>
    <!--ここまでメニュー-->
  </header>
</template>

<style>
header {
  width: 100%;
  background-image: linear-gradient(
    90deg,
    rgba(224, 162, 8, 1),
    rgba(255, 242, 58, 1)
  );
  position: relative; /* ウィンドウを基準に画面に固定 */
  top: 0; /* 上下の固定位置を上から0pxにする */
  left: 0; /* 左右の固定位置を左から0pxにする */
  box-sizing: border-box; /* padding分を含んで幅を100%にするため */
}
.header-title {
  text-align: center;
  box-sizing: border-box;
  color: #333333;
  padding: 10%;
}
.menu-btn {
  /*通常時のメニューボタンの設定*/
  position: fixed;
  top: 10px; /*上に固定*/
  right: 10px; /*右に固定*/
  display: flex;
  height: 70px; /*高さ*/
  width: 70px; /*幅*/
  padding: 20px 20px; /* ボタンに上下左右それぞれ余白を指定 */
  box-sizing: border-box; /* padding分を含んで幅を100%にするため 666*/
  justify-content: center; /*中央揃え*/
  align-items: center;
  z-index: 90;
  background-color: transparent;
}
.menu-btn span,
.menu-btn span:before,
.menu-btn span:after {
  content: "";
  display: block;
  height: 3px;
  width: 25px;
  border-radius: 3px;
  background-color: #111111;
  position: absolute;
  transition: all 0.5s; /*やんて アニメーション設定*/
}
.menu-btn span:before {
  bottom: 8px;
}
.menu-btn span:after {
  top: 8px;
}
#menu-btn-check:checked ~ .menu-btn span {
  background-color: rgba(
    255,
    255,
    255,
    0
  ); /*メニューオープン時は真ん中の線を透明にする*/
}
#menu-btn-check:checked ~ .menu-btn span::before {
  bottom: 0;
  transform: rotate(45deg);
}
#menu-btn-check:checked ~ .menu-btn span::after {
  top: 0;
  transform: rotate(-45deg);
}
#menu-btn-check {
  display: none;
}
.menu-content {
  width: 30%; /*やんて ここを30％に変える*/
  height: 100%;
  position: fixed;
  top: 0;
  left: 100%; /*leftの値を変更してメニューを画面外へ*/
  z-index: 80;
  background-image: linear-gradient(
    90deg,
    rgba(224, 162, 8, 1),
    rgba(255, 242, 58, 1)
  );
  transition: all 0.5s; /*アニメーション設定*/
}
.menu-content ul {
  padding: 70px 10px 0;
}
.menu-content ul li {
  border-bottom: solid 1px #333333;
  list-style: none;
}
.menu-content ul li a {
  display: block;
  width: 100%;
  font-size: 15px;
  box-sizing: border-box;
  color: #333333;
  font-family: "Itim", cursive;
  font-style: italic;
  text-decoration: none;
  padding: 9px 15px 10px 0;
  position: relative;
}
.menu-content p {
  display: block;
  width: 100%;
  font-size: 15px;
  box-sizing: border-box;
  color: #333333;
  text-decoration: none;
  padding: 10px 15px 0px 0;
  position: relative;
}
.menu-content ul li a::before {
  content: "";
  width: 7px;
  height: 7px;
  border-top: solid 2px #333333;
  border-right: solid 2px #333333;
  transform: rotate(45deg);
  position: absolute;
  right: 11px;
  top: 16px;
}
#menu-btn-check:checked ~ .menu-content {
  left: 70%; /*やんて ここを70％に変える*/ /*メニューを画面内へ*/
}
</style>
