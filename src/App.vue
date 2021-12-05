<template>
    <div class="container-fluid">
      <Navbar />
      <div>
        <b-row>
          <b-col cols="3">
            <Sidebar titulo="Carrito" />
          </b-col>
          <b-col cols="9">
            <CardsContainer 
              :productos="productos"
            />
            <Login />
            <Registro />
          </b-col>
        </b-row>
      </div>
    </div>
</template>

<script>
import productos from './assets/data/productos.json'

import Navbar from './components/Navbar.vue'
import Sidebar from './components/Sidebar.vue'
import CardsContainer from './components/CardsContainer.vue'
import Login from './components/Login.vue'
import Registro from './components/Registro.vue'

  export default {
    name: "App",
    components:{
      Navbar,
      Sidebar,
      CardsContainer,
      Login,
      Registro
    },
    data() {
      return {
        productos
      }
    }
  } 
</script>

<style scoped>

</style>