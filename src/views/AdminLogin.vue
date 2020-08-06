<template>
  <div class="about">
    <div class="one">
      <div class="one1">
        <h2>Login to dashboard</h2>
      </div>
      
      <div class="one2">
        <form @submit.prevent="adminLogin">
          <label for="Username"><h6>Email</h6> </label><br>
          <input type="text" placeholder="Admin" v-model="adminDetails.email"><br>
          <label for="password"><h6>Password </h6> </label><br>
          <input type="text" placeholder="******" v-model="adminDetails.password">
          <div class="center">
            <input type="submit" value="Submit" >
          </div>
          
        </form>
        
      </div>
    </div>
  </div>
</template>

<script>
import axios from 'axios'
export default {
    data(){
      return{
        adminDetails:{
          email:'',
          password:''
        }
      }
    },
    methods:{
      adminLogin(){
       const formData=new FormData();
       formData.append('email',this.adminDetails.email);
       formData.append('password',this.adminDetails.password);
       axios.post("https://srms-project.herokuapp.com/api/login",formData).then(res=>{
          console.log(res);
          window.location.href="http://localhost:8080/"
       });
     }
    }
}
</script>

<style scoped>
  .one{
    margin-left: 30%;
    margin-right: 30%;
    margin-top: 100px;
    margin-bottom: 100px;
  }
  .one1{
    text-align: center;
  }
  .one1 h2{
    color: #424B5F;
    font-size: 36px;
    margin-bottom: 30px;
  }
  .one2 label{
    color: #424B5F;
  }
  .one2 input{
    width: 100% !important;
    margin-top: 0px !important;
    margin-bottom: 30px;
    background: #FFFFFF;
    border: 2px solid #E0E0E0;
    border-radius: 4px;
    padding: 5px 10px;
  }
  .btn1{
    width: 40% !important;
    background: #698AFE;
    border-radius: 4px;
    border: none;
    padding-top: 10px;
    padding-bottom: 10px;
    color: #FFFFFF;
    margin-top: 10px;
  }
  .center{
    text-align: center;
  }
  .center input{
    width: 100% !important;
    background: #424B5F;
    border-radius: 4px;
    border: none;
    padding-top: 10px;
    padding-bottom: 10px;
    color: #FFFFFF;
    margin-top: 10px !important;
  }

  @media (max-width:567px){
    .one{
    margin-left: 20px;
    margin-right: 20px;
    margin-top: 100px;
    margin-bottom: 100px;
  }
  }


  @media (min-width:568px) and (max-width:768px){
    .one{
    margin-left: 20% !important;
    margin-right: 20% !important;
    margin-top: 100px;
    margin-bottom: 100px;
  }
  }

  @media (min-width:769px) and (max-width:1200px){

    .one{
    margin-left: 20% !important;
    margin-right: 20% !important;
    margin-top: 100px;
    margin-bottom: 150px;
  }
  }
</style>
