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
  </div>
</template>

<script>
import Navbar from './components/Navbar'

export default {
  name: 'App',
  components: {
    Navbar
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
}
</style>
