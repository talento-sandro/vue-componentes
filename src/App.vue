<template>
  <div id="app">
    <center>
      <img alt="Vue logo" src="./assets/logo.png"> <br/>
      <contador/>  <contador/>  <contador/> <contador/> <contador/> <br>
      <h2>Listado de planes de Cursos de Programación</h2>

      <div class="planes">
  <!--  <plan nombre="Plan 1  -  Principiante"/>
        <plan nombre="Plan 2  -  Intermedio"/>
        <plan nombre="Plan 3  -  Avanzado"/>
        <plan nombre="Plan 4  -  Hackers"/>
        <plan/> 
        <plan v-for="pla in planes" :nombre="pla" :key="pla"/> -->
        <planes />
      </div>
    </center>
  </div>
</template>

<script>
import Contador from './components/Contador'
import Planes from './components/Planes'
export default {
  name: 'App',
  components: {
  Contador,
  Planes
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
}
</style>

