<template>

  <b-navbar toggleable="lg" type="dark" variant="dark">
    <b-navbar-brand href="#">MiTienda</b-navbar-brand>

    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

    <b-collapse id="nav-collapse" is-nav>
      <b-navbar-nav>
        <b-nav-item href="#">Inicio</b-nav-item>
      </b-navbar-nav>

      <!-- Right aligned nav items -->
      <b-navbar-nav class="ml-auto">

        <b-nav-item href="#">Login</b-nav-item>
        <b-nav-item href="#">Registro</b-nav-item>

      </b-navbar-nav>
    </b-collapse>
  </b-navbar>



</template>

<script>
    export default {
        name: "Navbar",
        
    }
</script>

<style lang="scss" scoped>

</style>