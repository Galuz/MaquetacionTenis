<template>
  <div id="app">
    <header>
      <Navbar class="navbar-component"></Navbar>
      <div class="title">
        <h1>Las mejores raquetas para <br> jugar <strong>Tennis</strong></h1>
        <button>ACERCA DE NOSOTROS</button>
      </div>
    </header>
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
        font-family: 'HelveticaNeue-Bold';
        margin-top: 32px;
        padding: 15px 30px;
        background-color: transparent;
        border: 1px solid #fff;
        border-radius: 26.5px;
        color: #fff;
      }
    }
  }
}
</style>
