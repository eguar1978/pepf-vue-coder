<template>
    <div>
        <h1>Carrito</h1>        
        <CardsProducto 
          :producto="{articulo: 'Harina', precio: 41, cantidad: 2}"
          textButton="Comprar"
        />
    </div>
</template>

<script>
import CardsProducto from './CardsProducto.vue'

    export default {
        name: "Sidebar",
        props: {
            titulo: String,
        },
        components: {
            CardsProducto,
        }
    }
</script>

<style scoped>

</style>