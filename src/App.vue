<template>
  <div class="therapy">

    <NavBar/>
    <TherapyPage />
  </div>
</template>

<script>
import NavBar from './components/NavBar.vue';
import TherapyPage from './pages/Therapy.vue';
export default {
  name: 'App',
  components: {
    TherapyPage,
    NavBar,
}
}
</script>

<style>
*{
  box-sizing: border-box;
  accent-color: #A180D6; 
  margin: 0;
  padding: 0;
}
button{
  background-color: #868CD1;
  border: none;
  cursor: pointer;
}
body{
  background-color: #EEEFFF;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}
.therapy{
  display: flex;

}
</style>
