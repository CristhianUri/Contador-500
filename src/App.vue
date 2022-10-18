<template>
  <div class="container">
    <div class="center bg-warning text-center">Crishtian Uriel Castro Rosales </div>
    <img src="./assets/logo.svg" alt="Logo VUE" width="125" height="125" />
    <small>
      <h1>Hola desde VUE.js 3</h1>
    </small>
    <hr />

    <h2>Contador {{ contador }}</h2>
    <button @click="incrementar()" type="button" class="btn btn-outline-success btn-sm">+1</button>
    <button @click="disminuir()"   type="button" class="btn btn-outline-danger btn-sm">-1</button>
    <button @click="reset()"       type="button" class="btn btn-outline-warning btn-sm">Reset</button>
    
  </div>


</template>

<style scoped>
.container {
  text-align: center;
}
small {
  color: #666;
}
h1 {
  font-weight: bolder;
}
h2 {
  font-size: 2.5rem;
}
button {
  cursor: pointer;
  font-size: 1.5rem;
  margin: 0px 8px;
}
</style>
<script>
  export default {
    data: () => ({
      contador: 500,
    }),
    methods: {
      saludar() {
        console.log("Hola !");
      },
      incrementar() {
        this.contador++;
      },
      disminuir() {
        this.contador--;
      },
      reset() {
        this.contador = 500;
      },
    },
  };
  </script>