<template>
  <div class="container_s">
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
    <NuxtLink to = "../"><li>Home</li></NuxtLink>
    <NuxtLink to = "/articles"><li>Design</li></NuxtLink>
    <NuxtLink to = "/articles"><li>Markup Language</li></NuxtLink>
    <NuxtLink to = "/articles"><li>Programing Language</li></NuxtLink>
    </ul>
  </div>
</nav>
        <img src="~/assets/ym2t.png" class ="logo">
    </header>
        <body>
          <div class = "cts-article">
          <div class = "article-head">
            <h2 class="article-t">What is #ym2t / #ym2tとは</h2>
            <p class = "article-ymd">2020/3/20</p>
          </div>
            <p class="article-c">
             <img src = "../../assets/thumbnails/001.png">
             <span class="article-cts">
             みなさんこんにちは！#ym2tのやまもとです。
             今回はこの謎サイト<b>“#ym2t”</b>の外観を説明させていただきます！
            <h3>What is #ym2t</h3>
            #ym2tはデザイン、マークアップ言語からプログラミング言語までを発信するパブリックメディアです。
             </span>
            </p>
          </div>
        </body>
      </div>
  </div>
</template>

<script>
export default {
  data: () => {
    return {
      imgSrc: '~/assets/ym2t.png'
    };
  }
}
</script>



<style>
@media screen and (max-width:767px) { 

.d768{
  display: none;
}

.container_s {
  margin: 0 auto;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  background: #fff;
  z-index: -100;
  font-family: 'Noto Sans JP', sans-serif;
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

.cts-article{
  padding-bottom: 30px;
}

.article-head{
  display: block;
  margin-top: 80px;
  padding-bottom: 70px;
}

.article-t{
  display: block;
  position: absolute;
  margin-top: 22vw;
  left: 20px;
  margin: auto;
  color: #282828;
  font-weight: 900;
  font-family: 'Noto Sans JP', sans-serif;
}

.article-ymd{
  display: block;
  position: absolute;
  left: 20px;
  margin-top: 32px;
  color: #707070;
  font-size: 0.9rem;
  font-weight: bold;
}

.article-c{
  display: block;
  width: 100vw;
}

.article-c img{
  display: block;
  width: 100%;
}

.article-c h3{
  padding: 10px 10px 10px 15px;
  background: #2d73ff;
  color: #fff;
  margin: 15px 0 15px 0;
}

.article-cts::before{
  content: "";
  position: absolute;
  width: 20vw;
  height: 2px;
  background:#2d73ff;
  top: -4.5vw;
  left: 35vw;
}

.article-cts{
  display: block;
  position: relative;
  width: 90%;
  height: auto;
  margin: auto;
  margin-top: 10vw;
  text-align: left;
  word-wrap: break-word;
  font-weight: 300;
  line-height: 1.8;
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
  font-family: 'Source Sans Pro','Avenir','Helvetica Neue','Helvetica','Arial','Hiragino Sans','ヒラギノ角ゴシック',YuGothic,'Yu Gothic','メイリオ', Meiryo,'ＭＳ Ｐゴシック','MS PGothic';
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
  font-family: 'Source Sans Pro','Avenir','Helvetica Neue','Helvetica','Arial','Hiragino Sans','ヒラギノ角ゴシック',YuGothic,'Yu Gothic','メイリオ', Meiryo,'ＭＳ Ｐゴシック','MS PGothic';
  color: #282828;
}

}

</style>
