<template>
    <div @click="count">{{count}}</div>    
</template>

<script>
    export default {
        name:Counter,
        data(){  
        return {
          count: 0
          }
        },
        computed:{
           count(){
               return this.$store.state.count
           }
        }
    }
</script>

