

<template>
  <div id="app">    

      <input v-model.number="count"> <br> <br>

      <div v-for="item in count"  v-bind:key="item"> 
        <button @click="increment">+</button>         
        <span >{{count}}</span>  
        <button @click="decrement">-</button>
      </div>
      <br><br> 
      


  </div>
</template>




<script>
  export default {
    name:'app',   
      data(){  
        return {
          count: 0
          }
        },
      computed: {
        increment(){
          return this.$store.state.count
        },
        decrement(){
          return this.$store.state.count
        } 
      }
  }
    

</script>