<template>
  <div id="app">
    <header>
      <Navbar class="navbar-component"></Navbar>
      <div class="title">
        <h1>Las mejores raquetas para <br> jugar <strong>Tennis</strong></h1>
        <button class="button-rounded button-white">ACERCA DE NOSOTROS</button>
      </div>
    </header>
    <section class="section-1">
      <span>TENNIS</span>
      <div>
        <h2>Raquetas.Accesorios.<br>Pelotas.</h2>
        <div>
          <p>Conoce nuestras raquetas y aprende a jugar <br> Tennis cómo un profesional.</p>
          <button class="button-rounded button-black">HISTORIA</button>
        </div>
      </div>
    </section>
    <section class="section-2">
      <Carousel 
        :perPageCustom="[[0, 1]]"
        :navigationEnabled="true"
        class="carousel-1">
        <Slide>
          <div class="slide-text">
            <h3>Nuestras <br> <strong>Raquetas</strong></h3>
            <p>Conoce nuestras raquetas y <br> aprende a jugar Tennis cómo un <br> profesional.</p>
          </div>
          <img src="@/assets/images/ball-color.jpg" alt="">
        </Slide>
        <Slide>
          <div class="slide-text">
            <h3>Nuestras <br> <strong>Raquetas</strong></h3>
            <p>Conoce nuestras raquetas y <br> aprende a jugar Tennis cómo un <br> profesional.</p>
          </div>
          <img src="@/assets/images/ball-color.jpg" alt="">
        </Slide>
        <Slide>
          <div class="slide-text">
            <h3>Nuestras <br> <strong>Raquetas</strong></h3>
            <p>Conoce nuestras raquetas y <br> aprende a jugar Tennis cómo un <br> profesional.</p>
          </div>
          <img src="@/assets/images/ball-color.jpg" alt="">
        </Slide>
        <Slide>
          <div class="slide-text">
            <h3>Nuestras <br> <strong>Raquetas</strong></h3>
            <p>Conoce nuestras raquetas y <br> aprende a jugar Tennis cómo un <br> profesional.</p>
          </div>
          <img src="@/assets/images/ball-color.jpg" alt="">
        </Slide>
    </Carousel>
    
    <Carousel
      :perPageCustom="[[0, 1], [992, 3]]"
      :navigationEnabled="true"
      class="carousel-2">
      <Slide>
        <img src="@/assets/images/racket.png" alt="">
      </Slide>
      <Slide>
        <img src="@/assets/images/racket.png" alt="">
      </Slide>
      <Slide>
        <img src="@/assets/images/racket.png" alt="">
      </Slide>
      <Slide>
        <img src="@/assets/images/racket.png" alt="">
      </Slide>
    </Carousel>
    </section>
    <section class="section-3"></section>
    <footer>
      <div>
        <div class="links">
          <a href="#">Inicio</a>
          <a href="#">Acerca de nosotros</a>
          <a href="#">Historia</a>
          <a href="#">Contacto</a>
        </div>
        <div class="social">
          <img src="@/assets/images/linkedin.svg" alt="">
          <img src="@/assets/images/group-24.svg" alt="">
          <img src="@/assets/images/group-25.svg" alt="">
          <img src="@/assets/images/group-22.svg" alt="">
          <img src="@/assets/images/group-26.svg" alt="">
        </div>
      </div>
      <img src="@/assets/images/tennisBall.svg" alt="">
    </footer>
  </div>
</template>

<script>
import Navbar from './components/Navbar'
import { Carousel, Slide } from 'vue-carousel';

export default {
  name: 'App',
  components: {
    Navbar,
    Carousel,
    Slide
  }
}
</script>

<style lang="scss" scoped>
#app{
  font-family: 'HelveticaNeue';
  header{
    padding: 0 16px;
    @media(min-width: 992px){
      padding: 0;
    }
    display: flex;
    flex-direction: column;
    background: url('assets/images/group@2x.png');
    background-size: cover;
    background-position: right;
    background-repeat: no-repeat;
    height: 785px;
    .navbar-component{
      width: 100%;
    }
    .title{
      position: absolute;
      top: 37.7%;
      left: 0;
      @media(min-width: 992px){
        left: 173px;
      }
      h1{
        font-size: 53px;
        color: #fff;
        line-height: 1.28;
        letter-spacing: -0.05px;
        margin: 0 16px 16px 16px;
        @media(min-width: 992px){
          margin: 0;
        }
        strong{
          font-family: 'HelveticaNeue-Bold';
          color: #cbe346;
        }
      }
      button{
        margin: 32px 16px 0 16px;
        @media(min-width: 992px){
          margin: 32px 0 0 0;
        }
      }
    }
  }
  .section-1{
    background-color: #f3f4f8;
    display: flex;
    flex-direction: column;
    padding: 32px 16px;
    @media(min-width: 992px){
      flex-direction: row;
      padding: 72px 0 67px 0;
    }
    span{
      line-height: 2;
      letter-spacing: 1.87px;;
      width: auto;
      font-family: 'HelveticaNeue-Medium';
      font-size: 15px;
      text-align: left;
      color: #cbe346;
      margin-bottom: 16px;
      @media(min-width: 992px){
        width: 174px;
        margin-left: 255px;  
        margin-bottom: 0;
        text-align: right;
      }
    }
    >div{
      width: 100%;
      @media(min-width: 992px){
        margin-left: 51px;
        margin-right: 168px;
      }
      h2{
        font-size: 32px;
        @media(min-width: 992px){
          font-size: 50px;
        }
        line-height: 1.14;
        letter-spacing: -0.06px;
        color: #1e2335;
        margin-bottom: 32px;
      }
      >div{
        display: flex;
        flex-direction: column;
        @media(min-width: 992px){
          flex-direction: row;
        }
        p{
          font-size: 18px;
          color: #787878;
          line-height: 1.78;
          letter-spacing: 0.51px;
          margin-bottom: 16px;
          @media(min-width: 992px){
            margin: 0;
          }
        }
        button{
          margin-left: auto;
          margin-right: auto;
          @media(min-width: 992px){
            margin-top: auto;
            margin-right: 0;
          }
        }
      }
    }
  }
  .section-2{
    display: flex;
    flex-direction: column;
    @media(min-width: 992px){
      flex-direction: row;
    }
    .carousel-1{
      width: 100%;
      @media(min-width: 992px){
        width: 530px;
      } 
      .slide-text{
        position: absolute;
        top: 38px;
        right: 71px;
        h3{
          font-size: 50px;
          color: #fff;
          line-height: 1.28;
          letter-spacing: -0.06px;
        }
        p{
          font-size: 18px;
          color: #fff;
          line-height: 1.67;
          letter-spacing: 0.51px;
        }
      }
      img{
        width: 100%;
        @media(min-width: 992px){
          width: 530px;
        }
      }
    }
    .carousel-2{
      margin: 16px 0;
      @media(min-width: 992px){
        width: calc(100% - 582px);
        margin: auto 0 auto 52px;
      }
      img{
        @media(min-width: 992px){
          width: 288px;
        }
        width: 100%;
      }
    } 
  }
  .section-3{
    background: url('assets/images/action-athlete-ball.jpg');
    background-size: cover;
    background-position: left;
    height: 586px;
    @media(min-width: 992px){
      background-position: center;
    }
  }
  footer{
    display: flex;
    padding: 32px 16px;
    height: 203px;
    background-color: #cbe346;
    @media(min-width: 992px){
      padding: 64px 63px 58px 78px;
    }
    >div{
      display: flex;
      flex-direction: column;
      .links{
        margin-bottom: 13px;
        a{
          color: #2b3049;
          font-size: 13px;
          margin: 16px;
          letter-spacing: 1.14px;
          line-height: 37px;
          &:first-child{
            margin-left: 0;
          }
          &:hover,
          &:focus{
            font-family: 'HelveticaNeue-Bold';
          }
        }
      }
      .social{
        margin-top: auto;
        @media(min-width: 992px){
          margin-top: 0;
        }
        img{
        margin: 0 6px;
          &:first-child{
            margin-left: 0;
          }
        }
      }
    }
    >img{
      margin-left: auto;
    }
  }
}
</style>
