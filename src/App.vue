<template>
  <div id="app">
  
    <Counter />
   
  </div>
</template>

<script>
import Counter from './components/Counter'

export default {
  
  name: 'App',
  components:{
    Counter
  },
  data(){
    return{
 }
  },
}
</script>
<style scoped>
#app{
  max-width: 80%;
  background-color: #eee;
  height: 100vh;
  margin: auto;
  box-shadow: 0 0 4px black;
  padding: 1rem;
}


</style>

