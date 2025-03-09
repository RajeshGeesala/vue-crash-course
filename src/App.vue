<template>
  <div class="container">
    <div class="grid">
      <div class="col"><p class="h3 text-success fw-boled"> Lorem, ipsum dolor sit amet consectetur adipisicing elit. Fuga, deserunt laborum totam rerum, minus natus ducimus expedita earum officia cupiditate distinctio illo rem, a porro? Consequuntur libero natus tempore at?</p>
      <CustomerDetail name="Rajesh" age="26" designation="Engineer"/> 
    <EmployeeDetail/>
  <CounterComponent/>
<FunctionParam/> </div>
    </div>
  </div>
</template>

<script>

import CounterComponent from './components/CounterComponent.vue';
import CustomerDetail from './components/CustomerDetail.vue';
import EmployeeDetail from './components/EmployeeDetail.vue';
import FunctionParam from './components/FunctionParam.vue';


export default {
  name: 'App',
  components : {
    CustomerDetail, // Add Customers to the components object
    EmployeeDetail,
    CounterComponent ,
    FunctionParam
  }

}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #e90606;
  margin-top: 60px;
}
</style>
