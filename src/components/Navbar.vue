<template>
  <div class="tennis-nav">
    <b-navbar toggleable="lg" type="dark">
    <b-navbar-brand href="#">
        <img src="@/assets/images/tennisBall.svg" alt="tennis-ball">
    </b-navbar-brand>
    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
    <b-collapse id="nav-collapse" is-nav>
      <b-navbar-nav>
        <b-nav-item href="#">Inicio</b-nav-item>
        <b-nav-item href="#">Acerca de nosotros</b-nav-item>
        <b-nav-item href="#">Historia</b-nav-item>
        <b-nav-item href="#">Contacto</b-nav-item>
      </b-navbar-nav>
      <!-- Right aligned nav items -->
      <b-navbar-nav class="ml-auto">
        <b-nav-item href="#">ES</b-nav-item>
        <b-nav-item href="#">EN</b-nav-item>
      </b-navbar-nav>
    </b-collapse>
  </b-navbar>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="stylus" scoped>

</style>