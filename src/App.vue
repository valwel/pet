<template>
  <section class="section">
    <div class="header">
      <div class="logo">
        <img src="../src/assets/logo.jpg" alt="" class="logo__icon">
        <div class="logo__item">antools.</div>
      </div>
      <div class="menu">
        <ul class="menu__nav">
          <li class="menu__nav-item">Home</li>
          <li class="menu__nav-item">Categories</li>
          <li class="menu__nav-item">My Collections</li>
          <li class="menu__nav-item">Blog</li>
        </ul>
      </div>
      <div class="autoriz">
        <button class="button">Login</button>
        <button class="button">Sign Up</button>
      </div>
    </div>

    <div class="first-section">
      <div class="info">
        <div class="info__header"><p>Awesome too ls for</p> <p>Designer & Developer<span>.</span></p>
        </div>
        <div class="info__text">Antool is a web collection of information on paid or free Design and Development tools</div>
        <div class="search">
          <img src="@/assets/search.svg" alt="" class="search__icon">
          <input type="text" class="search__input" placeholder="find more than 430+ tools...">
          <button class="search__button button">Search</button>
        </div>
      </div>

      <div class="social">
        <div class="social__network">
          <img src="@/assets/facebook.png" alt="">
        </div>
        <div class="social__network">
          <img src="@/assets/instagram.png" alt="">
        </div>
        <div class="social__network">
          <img src="@/assets/twitter.png" alt="">
        </div>
      </div>
    </div>
  </section>
</template>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  // text-align: center;
  color: #fff;
}

/* Убираем внутренние отступы */
ul[class],
ol[class] {
  padding: 0;
}

/* Убираем внешние отступы */
body,
h1,
h2,
h3,
h4,
p,
ul[class],
ol[class],
li,
figure,
figcaption,
blockquote,
dl,
dd {
  margin: 0;
}

/* Удаляем стандартную стилизацию для всех ul и il, у которых есть атрибут class*/
ul[class],
ol[class] {
  list-style: none;
}

/* Элементы a, у которых нет класса, сбрасываем до дефолтных стилей */
a:not([class]) {
  text-decoration-skip-ink: auto;
}

/* Наследуем шрифты для инпутов и кнопок */
input,
button,
textarea,
select {
  font: inherit;
}

$grey: #283036;
$dark: #1E252B;
$orrange: #FF6E30;
$dim-white: rgb(255, 255, 255, .55);
$semi-dim-white: rgb(255, 255, 255, .78);
$bright-white: rgb(255, 255, 255, .9);
$border: 1px solid #000000;
$shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
$radius: 8px;

html {
  background-color: $dark;
  background-image: url(../src/assets/Illustration.png);
  background-repeat: no-repeat;
  background-position: right bottom;
  min-width: 1440px;
  min-height: 700px;
}

.section{
margin: 26px 108px;
}

.header{
  display: flex;
  justify-content: space-between;
  align-items: center;
  
}

.logo{
    display: flex;
    align-items: center;
    &__icon{
      width: 38px;
      height: 38px;
      border-radius: $radius+1;
      border: $border;
      box-shadow: $shadow;
    }
    &__item{
      margin-left: 12px;
      font-size: 22px;
      font-weight: bold;
      color: $bright-white;
    }
  }

  .menu{
    
    &__nav{
      display: flex;
      &-item{
        font-size: 16px;
        color: $dim-white;
      }
      &-item:nth-child(n+2){
        margin-left: 25px;
      }
    }
  }
  .button{
    color: #fff;
    background-color: $orrange;
    box-sizing: border-box;
    border: $border;
    box-shadow: $shadow;
    border-radius: $radius;
    height: 48px;
    width: 118px;
    cursor: pointer;
  }
  .button:nth-child(1){
    background-color: $dark;
    border: 0px;
    box-shadow: 0px 0px 0px;
    color: $dim-white;
    margin-right: 2px;
  }


  .first-section{
    margin-top: 104px;
    width: 600px;
    height: 354px;
  }

  .info{
    &__header{
      font-size: 50px;
      color: $bright-white;
      span{
        color: $orrange;
      }
    }
    &__text{
      margin-top: 30px;
      width: 487px;
      height: 60px;
      font-size: 18px;
      color: $dim-white;
    }
  }

  .search{
    display: flex;
    margin-top: 60px;
    border-radius: 15px;
    overflow: hidden;
    min-width: 500px;
    padding: 8px 11px 8px 18px;
    box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
    background: $grey;
    &__button{
      margin-left: 11px;
    }
    &__input{
      background: transparent;
      border: none;
      outline: none;
      color: $bright-white;
      flex-grow: 1;
      &:hover{
        border: none;
        outline: none;
      }
    }
    &__icon{
      margin-right: 11px;
    }
  }

  .social{
    display: flex;
    margin-top: 110px;
    &__network{
      width: 58px;
      height: 58px;
    }
  }

</style>
