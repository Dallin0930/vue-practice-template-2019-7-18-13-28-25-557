<template>
  <div class="other">
     <input v-model.number="count" placeholder="0" > <br> <br>

      <div v-for="item in count "  v-bind:key="item"> 
              <button @click="increment">+</button>         
              <span >{{count}}</span>  
              <button @click="decrement">-</button>
      </div><br><br> 
     <input placeholder="0">{{sunCount}}
  </div>
</template>


<script>
export default {
  name: 'counter',
  props: {
    msg: String
  }
}
</script>

