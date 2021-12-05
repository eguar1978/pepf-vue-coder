<template>
  <b-row  cols="1" cols-sm="2" cols-md="3" cols-lg="4">
          <b-col class="mb-3"  v-for="(producto, i) in productos" :key="i">
            <CardsProducto 
              :producto="producto"
              textButton="Agregar"
            />
          </b-col>
  </b-row>
</template>

<script>
import CardsProducto from './CardsProducto.vue'

  export default {
    name: "CardsContainer",
    props: {
      productos: Array
    },
    data() {
      return {
        fields: ['articulo', 'precio', 'cantidad'],
      }
    },
    components: {
      CardsProducto,
    }
  }
</script>