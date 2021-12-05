<template>

    <div>
        <b-card no-body>
            <b-card-body>
                <h5> 
                    {{ producto.articulo }} 
                </h5>
                <b-card-text>
                    Precio: {{ producto.precio }}
                </b-card-text>
                <b-card-text>
                    Cantidad: {{ producto.cantidad }}
                </b-card-text>

                <b-button href="#" variant="primary">{{ textButton }}</b-button>
            </b-card-body>
        </b-card>
    </div>

</template>

<script>
    export default {
        props: {
            producto: Object,
            textButton: String
        }
    }
</script>

<style scoped>

</style>