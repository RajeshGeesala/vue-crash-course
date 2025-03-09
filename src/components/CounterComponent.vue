<template>
    <h1>Counter  </h1>
    <button @click="increment">+</button>{{ COUNT }} <button @click="decrement">-</button>
</template>
<script>
export default {
    name : "CounterComponent",
    data : function ( ){
   return {  COUNT : 0}    },
   methods : {
   increment : function (){
    
     this.COUNT = this.COUNT + 1 
   },
   decrement : function () {
    if(this.COUNT === 0){
      return  alert("Value Should not be negative")
    }
    this.COUNT = this.COUNT -1
   }   
   }
}
</script>