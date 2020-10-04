<template>
  <div id="app">
    <header>
      <Navbar class="navbar-component"></Navbar>
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
    background: url('assets/images/group@2x.png');
    background-size: cover;
    background-position: right;
    background-repeat: no-repeat;
    height: 785px;
  }
  .navbar-component{
    width: 100%;
  }
}
</style>
