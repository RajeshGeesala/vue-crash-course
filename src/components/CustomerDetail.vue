 <template>
  <section>
    <h1>Customers</h1>
    <h2> name :{{ name }}</h2>
    <h2>age : {{  age }}</h2>
    <h2>designation : {{  designation }}</h2>
  </section>
</template>

<script >
export default {
  name : "CustomerDetail",
  props : {
    name : {type : String , required  : true},
    age : {type : Number , required  : true},
    designation : {type : String , required  : true}
  }
}

</script>
<style >
/* Your styles here */
</style>
