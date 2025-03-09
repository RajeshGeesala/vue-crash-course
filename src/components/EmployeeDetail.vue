<template>
  <section>
    <h1>Employee Information</h1>
    <div class="container">
      <div class="row">
        <div class="col">
          <div class="h3">Employee</div>
          <ul class="list-group">
            <li class="list-group-item">Name: {{ this.employe.name }}</li>
            <li class="list-group-item">Designation: {{ this.employe.designation }}</li>
            <li class="list-group-item">Age: {{ this.employe.age }}</li>
          </ul>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "EmployeeDetail",
  data() {
    return {
      employe  :{
        name: "Rajesh",
      designation: "Engineer",
      age: 24
      }
    };
  }
};
</script>

<style scoped>
/* Your styles here */
</style>
