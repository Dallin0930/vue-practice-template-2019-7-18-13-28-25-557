

<template>
  <div id="app">    

        <input v-model.number="count" placeholder="2" > <br> <br>

<!--        
        <button @click="increment">+</button>         
        <span >{{count}}</span> 
        <button @click="decrement">-</button>
       
  <ul id="example-1">
    <li v-for="item in count "  v-bind:key="item">
        {{ item }}  
    </li>
  </ul> -->

      <div v-for="item in count "  v-bind:key="item"> 
              <button @click="increment">+</button>         
              <span >{{count}}</span>  
              <button @click="decrement">-</button>
      </div>
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
        methods: {  
            increment(){
                this.count++;
            },
            decrement(){
                this.count--;  
            }
        }
    }


</script>