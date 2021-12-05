<template>
    <div>
        <hr>
        <h1>Registro</h1>
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
            <input 
                type="rePassword"
                placeholder="Repita la contraseña"
                class="form-control my-2"
                v-model="login.rePassword"
            >
            <input 
                type="email"
                placeholder="Ingrese su e-mail"
                class="form-control my-2"
                v-model="login.email"
            >
            <p>
            { 
                usuario: "{{ login.usuario }}",
                password: "{{ login.password }}",
                rePassword: "{{ login.rePassword }}",
                email: "{{ login.email }}"
            
            }</p>
            <button class="btn btn-dark">
                Registrar
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
                    password: "",
                    rePassword: "",
                    email: ""
                }
            }
        }
        
    }
</script>

<style scoped>

</style>