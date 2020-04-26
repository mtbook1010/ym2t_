<template>
  <div class="container">
    <div class = "d768">このウェブサイトはPC/タブレットに対応していません。スマートフォンでご利用ください。
    </div>
  <div class = "all">
    <head>
      <link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.12.1/css/all.css" integrity="sha384-v8BU367qNbs/aIZIxuivaU55N5GPF89WBerHoGA4QTcbUjYiLQtKdrfXnqAcXyTv" crossorigin="anonymous">
      <link href="https://fonts.googleapis.com/css2?family=Noto+Sans+JP:wght@300;700;900&family=Rubik:wght@400;700&display=swap" rel="stylesheet">
    </head>
    <header class="header">
      <nav role="navigation">
  <div id="menuToggle">
    <input type="checkbox" />
    <span></span>
    <span></span>
    <span></span>
    <ul id="menu">
    <NuxtLink to = "/articles" ><li>Design</li></NuxtLink>
    <NuxtLink to = "/articles" ><li>Markup Language</li></NuxtLink>
    <NuxtLink to = "/articles" ><li>Programing Language</li></NuxtLink>
    </ul>
  </div>
</nav>
        <img src="~/assets/ym2t.png" class ="logo">
    </header>
        <body>
          <div class="cts">
            <p>Hello,<br>Welcome to<br>#ym2t</p>
          </div>

          <div class="me">
            <img src="~/assets/me.gif">
          </div>

          <div class="cts-s">
          
          <p class="cts-c-text-st">Recommended Articles</p>
          <div class = "pop-c-t">
            おすすめの記事
          </div>

          <ul class="horizontal_scroll">
            <li>
            <div class = "cts-c-wrap cts-c-wrap1">
          <NuxtLink to = "/articles/001" >
            <img src = "../assets/thumbnails/001.png" >
            <div class = "cts-c-t">
            What is #ym2t / #ym2tとは
            </div>
            <div class = "cts-c-ymd">
            2020/3/20
            </div> 
          </NuxtLink>
            </div>
            </li>

            <li>
            <div class = "cts-c-wrap">
          <NuxtLink to = "/articles" >
            <img src = "../assets/thumbnails/002.png" >
            <div class = "cts-c-t">
            blender基礎 #1基本操作
            </div>
            <div class = "cts-c-ymd">
            2020/10/10
            </div>
          </NuxtLink>
            </div>
            </li>

            <li>
            <div class = "cts-c-wrap">
          <NuxtLink to = "/articles" >
            <img src = "../assets/thumbnails/003.png" >
            <div class = "cts-c-t">
            【2020】Google Fontsの使い方
            </div>
            <div class = "cts-c-ymd">
            2020/10/10
            </div> 
          </NuxtLink>
            </div>
            </li>
          </ul>

          <p class="cts-cate-text-st">Popular Categories</p>
          <div class = "pop-category">
            人気のカテゴリ
          </div>
          <div class="flexbox">
            <div class="item">
              <p class="title"><i class="fab fa-html5"></i>HTML5</p>
            </div>
            <div class="item">
              <p class="title"><i class="fab fa-js-square"></i>Vue.js</p>
            </div>
            <div class="item">
              <p class="title"><i class="fab fa-css3-alt"></i>CSS3</p>
            </div>
            <div class="item">
              <p class="title"><i class="fab fa-js-square"></i>Nuxt.js</p>
            </div>
            <div class="item">
              <p class="title"><i class="fab fa-adobe"></i>Photoshop</p>
            </div>
            <div class="item">
              <p class="title"><i class="fab fa-adobe"></i>illustrator</p>
            </div>
            <div class="item">
              <p class="title"><i class="fab fa-google"></i>GoogleFonts</p>
            </div>
          </div>
        </div>

        </body>
        <footer>
          <p class="footer"></p>
        </footer>
      </div>
  </div>
</template>

<script>
export default {
  data: () => {
    return {
      imgSrc: '~/assets/ym2t.png',
      imgSrc: '~/assets/me.gif',
      imgSrc: '~/assets/bars-solid.svg'
    };
  }
}

</script>



<style>
@media screen and (max-width:767px) { 

html{
  background: #2d73ff;
}

.d768{
  display: none;
}

.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  background: #2d73ff;
  z-index: -100;
}

.header{
  position: fixed;
  top: 0px;
  left: 0px;
  width: 100vw;
  height: 90px;
  text-align: center;
  z-index: 1000;
}

.header .logo {
    display: block;
    margin: auto;
    margin-top: -0.2rem;
    width: 120px;
}

.cts{
  position: fixed;
  top: 25vw;
  left: 10%;
  color: #fff;
  font-size: 10vw;
  font-weight: 700;
  text-align: left;
  font-family: 'Rubik', sans-serif;
  z-index: 99;
}

.me img {
  position: fixed;
  top: 22vw;
  right: 0px;
  width: 35%;
  z-index: 98;
}



.cts-s{
  display: block;
  position: relative;
  width: 100vw;
  height: 1000px;
  margin-top: 75vw;
  background: #fff;
  border-radius: 30px 30px 0 0;
  z-index: 99;
}

.cts-s-text-st , .cts-cate-text-st{
  text-align: left;
  font-size: 4vw;
  font-weight: 400;
  padding-top: 26px;
  padding-left: 27px;
  color: #909090;
  font-family: 'Rubik', sans-serif;
}

.cts-s-text-t{
  text-align: left;
  padding-left: 25px;
  width: 90%;
  font-size: 8vw;
  color: #282828;
  font-weight: bold;
  font-family: 'Rubik', sans-serif;
}

.cts-s-text{
  text-align: justify;
  padding-top: 8px;
  padding-left: 25px;
  width: 90%;
  font-size: 4.5vw;
  color: #505050;
  font-family: 'Rubik', sans-serif;
  font-weight: bold;
}

.links {
  padding-top: 15px;
}

.cts-c-text-st{
  text-align: left;
  font-size: 4vw;
  font-weight: 400;
  padding-top: 8vw;
  padding-left: 27px;
  color: #909090;
  font-family: 'Rubik', sans-serif;
}

.pop-c-t{
  text-align: left;
  margin-bottom: -3vw;
  padding-left: 25px;
  font-size: 8vw;
  font-weight: 900;
  color: #282828;
  font-family: 'Noto Sans JP', sans-serif;
}

.cts-c-wrap{
  position: relative;
  width: 70vw;
  background: #fff;
  margin: auto;
  margin-top: 30px;
  margin-right: 25px;
  padding-bottom: 5vw;
  border-radius: 30px;
  overflow: hidden;
  box-shadow: 0px 10px 30px 0px rgba(0, 0, 0, 0.1);
  transition: opacity 0.2s ease, box-shadow 0.2s ease;
  opacity: 1;
}

.cts-c-wrap1{
  margin-left: 25px;
}

.cts-c-wrap:hover {
  box-shadow: 0px 0px 10px 0px rgba(0, 0, 0, 0.1);
}

.cts-c-wrap img{
  width: 100%;
  background: #505050;
  border-radius: 30px 30px 0 0;
}

.cts-c-t {
  text-align: left;
  width: 85%;
  margin: auto;
  margin-top: 0.5rem;
  margin-bottom: 0.2rem;
  font-size: 0.9rem;
  font-weight: 700;
  color: #282828;
  font-family: 'Noto Sans JP', sans-serif;
}

.cts-c-ymd{
  font-size: 3vw;
  color: #707070;
  text-align: left;
  padding-left: 5vw;
}

.horizontal_scroll {
  overflow-x: scroll;
  -webkit-overflow-scrolling: touch;
  padding: 0 0 10vw 0;
  display: -ms-flexbox;
  display: flex; 
  -ms-overflow-style: none;    /* IE, Edge 対応 */
  scrollbar-width: none;       /* Firefox 対応 */
  }

.horizontal_scroll::-webkit-scrollbar{
  display: none;
}

.horizontal_scroll li{
  list-style-type: none;
}

.horizontal_scroll li a{
  -webkit-tap-highlight-color:rgba(0,0,0,0);
  text-decoration: none;
}

.pop-category{
  text-align: left;
  margin-bottom: -3vw;
  padding-left: 25px;
  font-size: 8vw;
  font-weight: 900;
  color: #282828;
  font-family: 'Noto Sans JP';
}

.flexbox{
  display: -webkit-flex;
  display: flex;
  -webkit-flex-direction: row;
  flex-direction: row;
  -webkit-flex-wrap: wrap;
  flex-wrap: wrap;
  justify-content: left;
  margin-top: 10px;
  margin-left:25px;
}

.item{
  display: block;
  margin-top: 20px;
}

.item p{
  font-weight: bold;
  color: #fff;
  padding: 15px;
  margin-right: 15px;
  background: #2d73ff;
  border-radius: 50px;
  box-shadow: 0px 5px 20px 0px rgba(0, 0, 0, 0.25);
}

.item p:hover{
  box-shadow: 0px 0px 10px 0px rgba(0, 0, 0, 0.25);
}

.fas , .fab{
  padding-right: 8px;
}

/*-----------------------------------------*/

#menuToggle {
    display: block;
    position: relative;
    top: 24px;
    left: 24px;
    z-index: 1;
    -webkit-user-select: none;
    -moz-user-select: none;
    -ms-user-select: none;
    user-select: none;
}

#menuToggle a
{
  text-decoration: none;
  color: #232323;
  
  transition: color 0.3s ease;
}

#menuToggle a:hover
{
  color: tomato;
}


#menuToggle input
{
  display: block;
  width: 40px;
  height: 32px;
  position: absolute;
  top: -7px;
  left: -5px;
  
  cursor: pointer;
  
  opacity: 0; /* hide this */
  z-index: 2; /* and place it over the hamburger */
  
  -webkit-touch-callout: none;
}

/*
 * Just a quick hamburger
 */
#menuToggle span {
    display: block;
    width: 33px;
    height: 4px;
    margin-bottom: 5px;
    position: relative;
    background: #282828;
    border-radius: 3px;
    z-index: 1;
    transform-origin: 4px 0px;
    transition: transform 0.5s cubic-bezier(0.77,0.2,0.05,1.0), background 0.5s cubic-bezier(0.77,0.2,0.05,1.0), opacity 0.55s ease;
}

#menuToggle span:first-child
{
  transform-origin: 0% 0%;
}

#menuToggle span:nth-last-child(2)
{
  transform-origin: 0% 100%;
}

/* 
 * Transform all the slices of hamburger
 * into a crossmark.
 */
#menuToggle input:checked ~ span
{
  opacity: 1;
  transform: rotate(45deg) translate(-2px, -1px);
  background: #232323;
}

/*
 * But let's hide the middle one.
 */
#menuToggle input:checked ~ span:nth-last-child(3)
{
  opacity: 0;
  transform: rotate(0deg) scale(0.2, 0.2);
}

/*
 * Ohyeah and the last one should go the other direction
 */
#menuToggle input:checked ~ span:nth-last-child(2)
{
  transform: rotate(-45deg) translate(0, -1px);
}

/*
 * Make this absolute positioned
 * at the top left of the screen
 */
#menu {
    position: absolute;
    top: 0px;
    width: 100vw;
    height: 105vh;
    margin-top: -53px;
    margin-left: -6.5vw;
    padding: 50px;
    padding-top: 125px;
    background: #fff;
    list-style-type: none;
    -webkit-font-smoothing: antialiased;
    transform-origin: 0% 0%;
    transform: translate(-100%, 0);
    transition: transform 0.5s cubic-bezier(0.77,0.2,0.05,1.0);
}

#menu li
{
  padding: 10px 0;
  text-align: left;
  font-size: 5.5vw;
  font-weight: bold;
  font-family: 'Rubik', sans-serif;
  color: #282828;
}

/*
 * And let's slide it in from the left
 */
#menuToggle input:checked ~ ul
{
  transform: none;
}

}

@media screen and (min-width:768px) { 
  .all{
    display: none;
  }

body{
    height: 100%;    /*高さを100％に設定*/
}

body{
  margin: 0;
  padding: 0;
  position: relative;
  min-width: 600px;  /*中央配置するボックスの横幅*/
  min-height: 400px;  /*中央配置するボックス縦幅*/
}

.d768{
  margin: 200px 0 0 -300px;  /*縦横の半分をネガティブマージンでずらす*/
  position: absolute;  /*body要素に対して絶対配置*/
  top: 50%;  /*上端を中央に*/
  left: 50%;  /*左端を中央に*/
  width: 600px;  /*横幅*/
  height: 400px;  /*縦幅*/
  background-color: #fff; /*横幅*/
  font-size: 1.5vw;
  font-weight: bold;
  font-family: 'Rubik', sans-serif;
  color: #282828;
}

}

</style>
