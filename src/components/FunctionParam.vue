<template>
  <section>
    <h1>FunctionParam</h1>
    <button @click="wish('Hii')">Hii</button> 
    <button @click="wish('Good Mrng')">Good Mrng</button>
    <button @click="wish('GoodNyt')">Good Nyt</button>
    <p>{{ msg }}</p>
  </section>
</template>

<script>
export default {
  name: "FunctionParam",
  data: function() {
    return {
      msg: "Hello, click below buttons to change text"
    };
  },
  methods: {
    wish: function(value) {
      this.msg = value;
    }
  }
}
</script>

<style scoped>
/* Your styles here */
</style>
