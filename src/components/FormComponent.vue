<template>
    <h1>Form Component </h1>
    <div class="container">
        <div class="row"><div class="col-md-3">
            <div class="card-header shadow-lg"><p>Registration Form</p>
                <p>{{ userDetails }}</p>
            <form @submit.prevent="register">
                <div class="mb-3">
                    <input class="form-control" v-model="userDetails.name"  type="text" placeholder="Name"/>
                </div>
                <div class="mb-3">
                    <input class="form-control"  v-model="userDetails.email" type="email" placeholder="Email"/>
                </div>
                <div class="mb-3">
                    <input class="form-control" type="password"  v-model="userDetails.password" placeholder="Password"/>
                </div>
                <div class="mb-3">
                    <input class="form-control"  type="submit" placeholder="Name"/>
                </div>

            </form></div>
        </div> </div>
    </div>
</template>
<script>
export default {
    name : "FormComponent",
    data  : ()  =>{
      return {
        userDetails : {
            name : "",
            email : "",
            password : ""
        }
      }
    },
    methods : {
           register : function () {
            console.log(this.userDetails)
           }
    }
}
</script>