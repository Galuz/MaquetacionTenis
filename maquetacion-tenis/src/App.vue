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
      :perPageCustom="[[992, 3]]"
      :paginationEnabled="false"
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
      left: 173px;
      h1{
        font-size: 53px;
        color: #fff;
        line-height: 1.28;
        letter-spacing: -0.05px;
        margin: 0;
        strong{
          font-family: 'HelveticaNeue-Bold';
          color: #cbe346;
        }
      }
      button{
        margin-top: 32px;
      }
    }
  }
  .section-1{
    background-color: #f3f4f8;
    display: flex;
    padding: 72px 0 67px 0;
    span{
      line-height: 2;
      letter-spacing: 1.87px;;
      width: 174px;
      font-family: 'HelveticaNeue-Medium';
      font-size: 15px;
      text-align: right;
      color: #cbe346;
      margin-left: 255px;
    }
    >div{
      margin-left: 51px;
      width: 100%;
      margin-right: 168px;
      h2{
        font-size: 50px;
        line-height: 1.14;
        letter-spacing: -0.06px;
        color: #1e2335;
        margin-bottom: 32px;
      }
      >div{
        display: flex;
        p{
          font-size: 18px;
          color: #787878;
          line-height: 1.78;
          letter-spacing: 0.51px;
          margin: 0;
        }
        button{
          margin-top: auto;
          margin-left: auto;
        }
      }
    }
  }
  .section-2{
    display: flex;
    .carousel-1{
      width: 530px;
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
        width: 530px;
      }
    }
    .carousel-2{
      width: calc(100% - 530px);
      margin: auto 0 auto 52px;
      img{
        width: 288px;
      }
    } 
  }
}
</style>
