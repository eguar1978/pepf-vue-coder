<template>
    <div>
        <hr>
        <h1>Login</h1>
        <form class="mt-3">
            <input 
                type="text"
                placeholder="Usuario"
                class="form-control my-2"
                v-model="login.usuario"
            >
            <input 
                type="password"
                placeholder="Contraseña"
                class="form-control my-2"
                v-model="login.password"
            >
            <p> { usuario: "{{ login.usuario }}", password: "{{ login.password }}"}</p>
            <button class="btn btn-dark">
                Ingresar
            </button>
        </form>
    </div>
</template>

<script>
    export default {
        name: "Login",
        components: {

        },
        data() {
            return {
                login: {
                    usuario: "",
                    password: ""
                }
            }
        }
        
    }
</script>

<style scoped>

</style>