<template>
  <div class="row align-items-center contenedor-login">
    <div class="col-12">
      <div class="card">
        <h2>Iniciar Sesión</h2>
        <form>
          <div class="contenedor-formulario">
            <label for="user">Usuario</label>
            <input type="text" class="form-control" id="user" aria-describedby="emailHelp" />
            <label for="pass">Contraseña</label>
            <div class="contenedor-formulario">
              <input type="password" class="form-control" id="pass" />
          <button v-on:click="inisiarSesion" type="submit" class="btn btn-primary">Iniciar Sesión</button>
            </div>
          </div>
        </form>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "LoginComponent",
  methods:{
    inisiarSesion(){
       this.$router.push({ path : '/principal' });
      console.log('hola mundo');
    },
  }
};
</script>

<style scoped>
.contenedor-login {
  background-image: url("../assets/monta.jpg");
    background-repeat: no-repeat;
    background-position: center;
    background-size: auto;
}
</style>